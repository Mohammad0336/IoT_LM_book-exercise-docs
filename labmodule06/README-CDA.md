# Constrained Device Application (Connected Devices)

## Lab Module 06

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-06-001 - Lab Module 06](https://github.com/orgs/programming-the-iot/projects/1#column-10488434).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

This implementation enhances the Constrained Device Application / CDA by incorporating MQTT for pub/sub communication. This 
integration allows the CDA to not only publish messages to an MQTT broker but also receive updates based on its specific 
subscriptions.

How does your implementation work?

Integrates an MQTT client into the CDA to establish a connection with an MQTT broker. This 
MQTT client allows subscriptions for receiving updates and adds an abstraction layer for MQTT 
functionality within the CDA.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/Abbas-Rizvi/iot-python-components

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/e5dea903-f45f-4885-83f0-271d5a058e99)

### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- PIOT-CFG-06-001

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/a6a4e304-5727-4c77-954d-020129f79898)

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- PIOT-CDA-06-001
![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/34c0e65d-8cc2-41d9-a495-3a277798959d)

- PIOT-CDA-06-002
![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/7bc1335f-1f87-40d7-a240-41d7c25df1fa)

- PIOT-CDA-06-003
![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/030f3ab4-d096-4f2c-bcda-7c9a27918f39)

EOF.
