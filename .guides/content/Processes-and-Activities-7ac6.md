
When an activity needs to start, Android checks if there’s already a process for that app. 
If one exists, Android runs the activity in that process. 
If one doesn’t exist, Android creates one.

![](.guides/img/39diagram.png)

When Android starts an activity, it calls its **onCreate()** method.

![](.guides/img/40diagram.png)

But there are still lots of things we don’t yet know about how activities function. How long does the activity live for? What happens when your activity disappears from the screen? Is it still running? Is it still in memory? And what happens if your app gets interrupted by an incoming phone call? We want to be able to control the behavior of our activities in a *whole range of different circumstances*, but how?
