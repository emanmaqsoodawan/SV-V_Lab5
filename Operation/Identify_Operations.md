| Operation ID | Operation | Purpose |
| --- | --- | --- |
| **OP-01** | `runSelfCheck` | Tests all sensors and control devices at startup to make sure everything works before doing anything else. |
| **OP-02** | `saveArtifactInfo` | Saves the artifact's ID along with its safe targets for temperature, humidity, light, and vibration. |
| **OP-03** | `checkDoor` | Keeps an eye on the door so active conservation only runs when the chamber is tightly closed. |
| **OP-04** | `readSensors` | Continuously checks the room's conditions, including climate, vibration, light, and power. |
| **OP-05** | `checkLimits` | Compares the latest sensor readings against the artifact's safe ranges to spot problems early. |
| **OP-06** | `fixTemperature` | Turns on the heater or cooler whenever the chamber gets too hot or too cold. |
| **OP-07** | `fixHumidity` | Turns on the humidifier or dehumidifier if the air gets too wet or too dry. |
| **OP-08** | `confirmStable` | Waits and checks the sensors to ensure a condition actually stays stable before marking it safe. |
| **OP-09** | `triggerProtection` | Dims lights and fires up backup controls if climate issues aren't fixed in time. |
| **OP-10** | `alertStaff` | Sends a quick warning to the museum team whenever something goes wrong or needs attention. |
| **OP-11** | `handleShaking` | Pauses risky actions right away if high vibrations or shocks are detected. |
| **OP-12** | `pauseOnOpenDoor` | Instantly pauses active climate control if someone opens the door during conservation. |
