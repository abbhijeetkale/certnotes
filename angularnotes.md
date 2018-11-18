As you can see here we’re using the factory method RouterModule.forRoot to handover our routing configuration.


Behaviour subjects. I wrote a blog about that.

import { BehaviorSubject } from 'rxjs/BehaviorSubject';
private noId = new BehaviorSubject<number>(0);
  defaultId = this.noId.asObservable();

newId(urlId) {
 this.noId.next(urlId);
 }
In this example i am declaring a noid behavior subject of type number. Also it is an observable. And if "something happend" this will change with the new(){} function.

So, in the sibling's components, one will call the function, to make the change, and the other one will be affected by that change, or vice-versa.

For example, I get the id from the URL and update the noid from the behavior subject.

public getId () {
  const id = +this.route.snapshot.paramMap.get('id');
  return id;
}

ngOnInit(): void {
 const id = +this.getId ();
 this.taskService.newId(id)
}
And from the other side, I can ask if that ID is "what ever i want" and make a choice after that, in my case if i want to delte a task, and that task is the current url, it have to redirect me to the home:

delete(task: Task): void {
  //we save the id , cuz after the delete function, we  gonna lose it
  const oldId = task.id;
  this.taskService.deleteTask(task)
      .subscribe(task => { //we call the defaultId function from task.service.
        this.taskService.defaultId //here we are subscribed to the urlId, which give us the id from the view task
                 .subscribe(urlId => {
            this.urlId = urlId ;
                  if (oldId == urlId ) {
                // Location.call('/home');
                this.router.navigate(['/home']);
              }
          })
    })
}

https://dzone.com/articles/design-patterns-in-expressjs
https://codehandbook.org/understanding-factories-design-pattern-in-node-js/
https://thejackalofjavascript.com/node-js-design-patterns/
https://medium.com/@kalin.chernev/reflecting-on-node-js-design-patterns-6cc6eaa584
https://blog.risingstack.com/fundamental-node-js-design-patterns/
https://github.com/rishabh115/engineering-blogs

https://blog.cloudboost.io/build-simple-shopping-cart-with-angular-4-observables-subject-subscription-part-2-2d3735cde5f

http://jasonwatmore.com/post/2018/06/25/angular-6-communicating-between-components-with-observable-subject

https://blog.angulartraining.com/rxjs-subjects-a-tutorial-4dcce0e9637f


https://medium.com/dailyjs/3-ways-to-communicate-between-angular-components-a1e3f3304ecb