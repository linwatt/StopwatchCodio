Very similar to onStop, we also need to check if the app was already running then we set running = true to set it running again.
```
@Override    
protected void onStart() {        	
	super.onStart();
	if (wasRunning) {        
		running = true;    
	}
}
```
