The **runTimer()** method will get a reference to the text view in the layout, format the contents of the seconds variable into hours, minutes, and seconds, and then display the results in the text view. If the running variable is set to true, it will increment the seconds variable. 

![](.guides/img/49code.png)

We need this code to keep looping so that it increments the seconds variable and updates the text view every second. We need to do this in such a way that we don’t block the main Android thread. Do this using a **Handler**.
