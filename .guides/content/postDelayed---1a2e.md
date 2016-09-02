The **postDelayed()** method works in a similar way to the post() method except that you use it post code that should be run in the future. 

The postDelayed() method takes two parameters: a Runnable and a long. 
- The Runnable contains the code you want to run in its run() method and 
- The long specifies the number of milliseconds you wish to delay the code by. The code will run as soon as possible after the delay.

![](.guides/img/51code.png)