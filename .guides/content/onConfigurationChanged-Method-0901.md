
![](.guides/img/8files.png)
![](.guides/img/7.png)

If Android encounters this type of configuration change, it makes a call to the **onConfigurationChanged(Configuration)** method instead of re-creating the activity: You can implement this method to react to the configuration change if you need to or just do nothing. 
```
public void onConfigurationChanged(Configuration config) {
	// do nothing here
}
```

The better way of dealing with configuration changes which you’ll use most often is to save the current state of the activity, and then reinstate it in the **onCreate()** method of the activity.  **onConfigurationChanged** seems to be buggy.  Issues with going from Landscape back to Portrait.


