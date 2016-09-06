![](.guides/img/13fixed.png)

The user starts the app, and clicks on the start button to set the stopwatch going. 

The **runTimer()** method starts incrementing the number of seconds displayed in the time_view text view. 

The user rotates the device. Android views this as a configuration change, and gets ready to destroy the activity. Before the activity is destroyed, **onSaveInstanceState()** gets called. 

The **onSaveInstanceState()** method saves the seconds and running values to a Bundle. 

**Android destroys the activity, and then re-creates it.**

The **onCreate()** method gets called, and the Bundle gets passed to it. The Bundle contains the values of the seconds and running variables as they were before the activity was destroyed. 

Code in the **onCreate()** method set the current variables to the values in the Bundle. 

The **runTimer()** method gets called, and the timer picks up where it left off. 

The stopwatch gets displayed on the device.




