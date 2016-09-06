Alternatively you can save the state.  To save the current state of the activity, you need to implement the **onSaveInstanceState()** method. 

![](.guides/img/9.png)

The **onSaveInstanceState()** method gets called before the activity gets destroyed, which means you get an opportunity to save any values you want to retain before they get lost. The **onCreate()** method gets passed to the Bundle as a parameter. 

This means that if you add the values of the 'running' and 'seconds' variables to the Bundle, the **onCreate()** method will be able to pick them up when the activity gets recreated. 

To do this, you use **Bundle methods** to add name/value pairs to the Bundle. 

```
bundle.put*("name", value)
```

