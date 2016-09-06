**The user starts the app, and clicks on the start button to set the stopwatch going.**
The **runTimer()** method starts incrementing the number of seconds displayed in the time_view text view.

![](.guides/img/24.png)

**Another activity appears in the foreground, leaving StopwatchActivity partially visible.**
The **onPause()** method gets called, wasRunning is set to true, running is set to false, and the number of seconds stops incrementing.

![](.guides/img/25.png)

**When StopwatchActivity returns to the foreground, the onResume() method gets called, running is set to true, and the number of seconds starts incrementing again.**

![](.guides/img/26.png)

