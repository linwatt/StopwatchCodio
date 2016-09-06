So far we’ve made the stopwatch stop if the Stopwatch app isn’t visible, and made it start again when the app becomes visible again. 

In addition to this, let’s get the stopwatch to stop if the activity is paused, and start again when the activity is resumed. 

So which lifecycle methods do we need to implement? We need to use onPause() and onResume() methods


![](.guides/img/23.png)