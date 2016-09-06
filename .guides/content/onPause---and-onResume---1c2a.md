![](.guides/img/22.png)

**1) The activity gets launched, and the onCreate() and onStart() methods run.**
At this point, the activity is visible, but it doesn’t have the focus.

**2) The onResume() method runs after the onStart() method. It gets called when the activity is about to move into the foreground.**
After the **onResume()** method has run, the activity has the focus and the user can interact with it.

**3) The onPause() method runs when the activity stops being in the foreground.**
After the **onPause()** method has run, the activity is still visible but doesn’t have the focus.

**4) If the activity moves into the foreground again, the onResume() method gets called.**
The activity may go through this cycle many times if the activity repeatedly loses and regains the focus.

**5) If the activity stops being visible to the user, the onStop() method gets called.**
After the **onStop()** method has run, the activity is no longer visible.

**6) If the activity becomes visible to the user again, the onRestart() method gets called, followed by onStart() and onResume().**
The activity may go through this cycle many times.

**7) Finally, the activity is destroyed.**
As the activity moves from running to destroyed, the **onPause()** method gets called before the activity is destroyed. The **onStop()** method usually gets called too.
