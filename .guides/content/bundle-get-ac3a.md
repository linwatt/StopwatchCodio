If the activity’s being re-created **and there’s been a prior call to onSaveInstanceState()**, the Bundle object used by onSaveInstanceState() will get passed to the activity: 

You can get values from Bundle by using methods of the form
```
bundle.get*("name");
```

![](.guides/img/12files.png)
![](.guides/img/11.png)