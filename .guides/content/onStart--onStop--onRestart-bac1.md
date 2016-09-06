An activity has a state of **stopped** if it’s completely hidden by another activity and isn’t visible to the user. The activity still exists in the background and maintains all state information. For example, when there’s a phone call. 

**onStart()** gets called when your activity becomes visible to the user.

**onStop()** gets called when your activity has stopped being visible to the user. This might be because it’s completely hidden by another activity that’s appeared on top of it, or because the activity is going to be destroyed. 

If **onStop()** is called because the activity’s going to be destroyed, **onSaveInstanceState()** gets called **before** onStop(). 

**onRestart()** gets called **after** your activity has been made invisible, **before** it gets made visible again.


![](.guides/img/14.png)