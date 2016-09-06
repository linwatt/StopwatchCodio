![](.guides/img/5.png)

**The activity gets launched.**
The activity object is created and its constructor is run.

**The onCreate() method runs immediately after the activity is launched.**
The onCreate() method is where any initialization code should go, as this method always gets called after the activity has launched and before it starts running.

**An activity is running when it’s visible in the foreground and the user can interact with it.**
This is where an activity spends most of its life.

**The onDestroy() method runs immediately before the activity is destroyed.**
The onDestroy() method enables you to perform any final clean up such as freeing up resources.

**After the onDestroy() method has run, the activity is destroyed.**
The activity ceases to exist.


