To update the stopwatch, we’re going to repeatedly schedule code using the Handler with a delay of 1,000 milliseconds each time. 

Each time the code runs, we’ll increment the seconds variable and update the text view. Using the **post()** and **postDelayed()** methods in this way means that the code will run as soon as possible after the required delay, which in practice means almost immediately. 

While this means the code will lag slightly over time, it’s accurate enough for the purposes of exploring the lifecycle methods in this chapter.

![](.guides/img/52code.png)
