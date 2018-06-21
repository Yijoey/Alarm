# Yi Zhao

## Alarm

The clock shows the time of day. Using buttons, the user can set the hours and minutes fields individually, and choose between 12 and 24-hour display.

It is possible to set one or two alarms. When an alarm fires, it will sound some noise. The user can turn it off, or choose to “snooze”. If the user does not respond at all, the alarm will turn off itself after 2 minutes. “Snoozing” means to turn off the sound, but the alarm will fire again after some minutes of delay. This “snoozing time” is pre-adjustable.

![Alt text](diagram-gmm.jpg)

| Scenario | set time and alarm |     ||
| ------------- |:-------------:| ----:|-----:|
| Triggering event | an operator set time | | |
| Actors | operator |||
| Related use cases | N/A |||
| Pre-condition  | time and alarm are not set yet |||
| post_condition | alarm is set successfully |||
| Flow of events | Actor                        | system ||
|   | 1.set hours                    |||
|   | 2. Set minutes |||
|   | 3. Choose 12/24 hours format        |||
|   | 4. Set snooze time                |||
|   | 5. Set alarm                    || |
|   |                          | 6. Play noise ||
|   | 7. Snooze                      || |
|   | 8. Turn off alarms        || |            
|Exception | step    |condition|    Action Description|        
|| 1a|    set wrong hour|    set an alarm and notify the operator to correct the problem 
|| 2a| set wrong minutes|     set an alarm and notify the operator to correct the problem 
|| 5a|    alarm failure|    set an alarm and notify the operator to correct the problem 

