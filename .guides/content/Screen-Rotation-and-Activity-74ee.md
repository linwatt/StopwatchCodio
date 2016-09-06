![](.guides/img/2.png)



When the user rotates the device, Android sees that the screen orientation and screen size has changed, and it destroys the activity, including any variables used by the **runTimer()** method. 

**StopwatchActivity** is then re-created. The **onCreate()** method runs again, and the **runTimer()** method gets called. 

As the activity has been re-created, the seconds and running variables are set to their default values.

When the device configuration changes, anything that displays a user interface needs to be updated to match the new configuration. 

If you rotate your device, Android spots that the screen orientation and screen size has changed, and classes this as a change to the device configuration. 

It destroys the current activity, and then re-creates it again so that resources appropriate to the new configuration get picked up.


