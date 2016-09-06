You override the **onStop()** method in the Android Activity class by adding the following method to your activity. Whenever you override one of the Android lifecycle methods, it’s important that you first call up the onStop()method in the superclass using: 
```
@Override    
protected void onStop() {        	
	super.onStop();        
	running = false;    
}
```

There are a couple of reasons for this:  
- First, you need to make sure that the activity gets to perform all of the actions in the superclass lifecycle method. 
- Second, Android will never forgive you if you bypass this step—it will generate an exception. We need to get the stopwatch to stop when the onStop() method is called. To do this, we need to set the value of the running boolean to false. So now the stopwatch stops when the activity is no longer visible. 

The next thing we need to do is get the stopwatch to start again when the activity becomes visible.
