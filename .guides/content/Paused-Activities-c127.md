**But what happens when an app is only partially visible?**

When an activity is visible but doesn’t have the focus, the activity is **paused**. This can happen if another activity appears on top of your activity that isn’t full-size or that’s transparent. 


![](.guides/img/21.png)

The activity on top has the focus, but the one underneath is still visible and is therefore paused. **An activity has a state of paused if it’s lost the focus but is still visible to the user. The activity is still alive and maintains all its state information.**


There are two lifecycle methods that deal with when the activity is paused and when it becomes active again: **onPause()** and **onResume()**: 

**onPause()** gets called when your activity is visible but another activity has the focus. 

**onResume()** is called immediately before your activity is about to start interacting with the user. 

If you need your app to react in some way when your activity is paused, you need to implement these methods.
