# Constrained Device Application (Connected Devices)

## Lab Module 08

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-08-001 - Lab Module 08](https://github.com/orgs/programming-the-iot/projects/1#column-10488501).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

The implementation involves creating a Python module named CoapServerAdapter. This module is designed to provide CoAP server functionality and host local resource implementations. 
The server has an option of two CoAP libraries: CoAPthon3 and aiocoap. CoapServerAdapter is connected into DeviceDataManager, establishing integration within the broader system. Additionally, two Python 
modules, GetSystemPerformanceResourceHandler and GetTelemetryResourceHandler are created to allow the CoAP OBSERVE specification, enabling the CoapServerAdapter to notify 
the GDA of new SensorData and SystemPerformanceData payloads.

How does your implementation work?

The implementation works by leveraging the CoAPthon3 or aiocoap libraries to establish CoAP server capabilities. CoapServerAdapter acts as the central component, managing local resources and bridging communication 
with DeviceDataManager. The new resource handler modules, such as GetSystemPerformanceResourceHandler and GetTelemetryResourceHandler, are essential for handling specific types of input data and enabling observation.
The UpdateActuatorResourceHandler module is made to allow communication from GDA to CDA by passing ActuatorData instances through PUT requests.


### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/Abbas-Rizvi/iot-python-components

### UML Design Diagram(s)

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/40afb017-a398-46b3-ab84-f535b1f68a40)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

N/A

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- PIOT-CDA-08-004

  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/c462db44-3a57-429a-8dd4-736ecd54e951)


EOF.
