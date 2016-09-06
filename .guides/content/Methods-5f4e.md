<table style="width:100%">
  <tr>
    <th>Method</th>
    <th>When it's called</th> 
    <th>Next Method</th>
  </tr>
  <tr>
    <td>onCreate()</td>
    <td>When the activity is first created. Use it for normal static setup, such as creating views. It also gives you a Bundle giving the previously saved state of the activity</td> 
    <td>onStart()</td>
  </tr>
  <tr>
    <td>onRestart()</td>
    <td>When your activity has been stopped just before it gets started again.
</td> 
    <td>onStart()</td>
  </tr>
    <tr>
    <td>onStart()</td>
    <td>When your activity is becoming visible. It’s followed by onResume() if the activity comes into the foreground, or onStop() if the activity is made invisible.

</td> 
    <td>onResume() or onStop()</td>
  </tr>
    <tr>
    <td>onResume()</td>
    <td>When your activity is in the foreground.
</td> 
    <td>onPause()</td>
  </tr>
    <tr>
    <td>onPause()</td>
    <td>When your activity is no longer in the foreground because another activity is resuming. The next activity isn’t resumed until this method finishes, so any code in this method needs to be quick. It’s followed by onResume() if the activity returns to the foreground, or onStop() if it becomes invisible.
</td> 
    <td>onResume() or onStop()</td>
  </tr>
    <tr>
    <td>onStop()</td>
    <td>When the activity is no longer visible. This can be because another activity is covering it, or because the activity’s being destroyed. It’s followed by onRestart() if the activity becomes visible again, or onDestroy() if the activity is going to be destroyed.
</td> 
    <td>onRestart() or onDestroy()</td>
  </tr>
</table>

