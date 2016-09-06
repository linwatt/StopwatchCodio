![](.guides/img/15.png)

**1) The activity gets launched, and the onCreate() method runs.**
Any activity initialization code in the **onCreate()** method runs. At this point, the activity isn’t yet visible, as no call to **onStart()** has been made.


**2) The onStart() method runs after the onCreate() method. It gets called when the activity is about to become visible.**
After the **onStart()** method has run, the user can see the activity on the screen.


**3) The onStop() method runs when the activity stops being visible to the user.**
After the **onStop()** method has run, the activity is no longer visible.


**4) If the activity becomes visible to the user again, the onRestart() method gets called followed by onStart().**
The activity may go through this cycle many times if the activity repeatedly becomes invisible and visible again.


**5) Finally, the activity is destroyed.**
The **onStop()** method will usually get called before **onDestroy()**, but it may get bypassed if the device is extremely low on memory.
