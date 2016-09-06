We’ll use the **onPause** and **onResume** methods to replace the calls to **onStop()** and **onStart()** that we’ve already implemented. 
```
@Override 
protected void onPause() { 	super.onPause(); 
	wasRunning = running; 
	running = false;
}
```

```
@Override 
protected void onResume() { 	super.onResume(); 
	if (wasRunning) { 
		running = true; 
	}
}
```

**Replace the onStop() and onStart() methods in your code with the onPause() and onResume() methods shown here.**
