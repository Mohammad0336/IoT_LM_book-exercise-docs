# Gateway Device Application (Connected Devices)

## Lab Module 08

Be sure to implement all the PIOT-GDA-* issues (requirements) listed at [PIOT-INF-08-001 - Lab Module 08](https://github.com/orgs/programming-the-iot/projects/1#column-10488501).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

The Java implementation involves a class named CoapServerGateway, acting as the CoAP server to host remote resources. Two new classes, UpdateSystemPerformanceResourceHandler and UpdateTelemetryResourceHandler, 
enable the CDA to execute PUT requests for SensorData and SystemPerformanceData to the GDA. GetActuatorCommandResourceHandler, allows the GDA to notify the CDA of actuation commands via CoAP OBSERVE. 

How does your implementation work?

This implementation works by using CoapServerGateway as the central component for CoAP server functionality and remote resource hosting. The class is adjusted to include specific resource handlers, like 
UpdateSystemPerformanceResourceHandler and UpdateTelemetryResourceHandler, facilitating PUT requests for SensorData / SystemPerformanceData. The GetActuatorCommandResourceHandler class supports GDA to CDA communication for
actuation commands through CoAP OBSERVE.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/Abbas-Rizvi/iot-java-components

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/6e97001e-52fd-4488-bc78-473849bef026)


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- PIOT-CFG-08-001

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/97e7efba-97f5-4edb-b836-2ea631eeba19)
![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/f7a0ea1c-daad-4302-8a83-9e2b39be5ea8)



### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- PIOT-GDA-08-004

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/fc7f11cd-56a0-4e94-b86d-8339aff0c3bf)


EOF.
