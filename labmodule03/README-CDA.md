# Constrained Device Application (Connected Devices)

## Lab Module 03

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-03-001 - Lab Module 03](https://github.com/orgs/programming-the-iot/projects/1#column-10488379).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

The implementation creates an environment to emulate sensors and or actuators within the application. 
It permits the generation of sensor measurements, such as temperature, humidity, and pressure, and allows them all to 
simulate actuation events.

How does your implementation work?

The implementation works with the utilization of data containers to support both data collection and actuation within the 
program. Following that, the establishment of sensor simulation for data storage and interfaces for data access is 
completed. Then it establishes connections between the sensors and the adapter manager, as well as between the actuators 
and respective adapter manager. A device data manager responsible for overseeing both existing and newly created managers, 
serves as the new handler class.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/Abbas-Rizvi/iot-python-components

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/cd95a7e6-7121-4829-91f9-06e825149877)

### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ActuatorDataTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/d96cf077-5bc8-4051-8d91-d1a5f7e89f53)

- SensorDataTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/6388ccd2-c121-4c8f-bf45-047a5667790a)

- SystemPerformanceDataTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/a029656a-1dc3-4fd4-942c-ea2470d1147c)

- HumiditySensorSimTaskTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/9062a916-9635-4ace-8c52-cdfd940aa0ad)

- PressureSensorSimTaskTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/a6ec5e5b-15b1-4310-af6b-8609ee1d69ed)

- TemperatureSensorSimTaskTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/4f7f116c-9ec9-4b2b-847f-ad8ac827f616)

- HumidifierActuatorSimTaskTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/0833cf4a-8764-40fa-85cd-2c17d984675f)

- HvacActuatorSimTaskTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/b5200c65-1e6d-4b9e-a448-6c5e1f818e45)

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SensorAdapterManagerTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/16546b6c-83c6-4e78-8cdf-e8e84dbbdd55)

- ActuatorAdapterManagerTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/76fae435-54ec-4369-9baa-0750f9029507)

- DeviceDataManagerNoCommsTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/5e2c0989-cdec-4601-908e-61934aa8adb0)

- ConstrainedDeviceAppTest.py

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/c68ac554-e1e1-4e4d-a114-649c5d25d186)



EOF.
