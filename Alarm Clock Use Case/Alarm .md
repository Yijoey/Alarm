# Alarm
![Alt text]（diagram-gmm.jpg）

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
