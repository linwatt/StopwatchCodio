- Use 'seconds' and 'running' to record the number of seconds passed and whether the stopwatch is running
```
private int seconds = 0;
private boolean running;
```

- When the Start button is clicked, start the stopwatch running:
```
running = true
```

- When the Stop button is clicked, stop the stopwatch running:
```
running = false
```
- When the Reset button is pressed, stop the stopwatch running, and set seconds to zero:
```
running = false;
seconds = 0;
```

Full code below:

![](.guides/img/48code.png)


