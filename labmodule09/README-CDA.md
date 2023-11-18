# Constrained Device Application (Connected Devices)

## Lab Module 09

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-09-001 - Lab Module 09](https://github.com/orgs/programming-the-iot/projects/1#column-10488503).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do?

The implementation aims to build a robust request/response data communication client for the CDA and GDA 
using the CoAP (Constrained Application Protocol). The goal is to demonstrate successful communication between the GDA and 
CDA utilizing this protocol, particularly with the server created in the previous module.

How does your implementation work?

The implementation involves adding a basic CoAP client abstraction layer into both the CDA and GDA. 
This layer facilitates sending CoAP requests (GET, POST, PUT, DELETE) to the GDA's CoAP server. The goal is to validate 
the functionality through successful communication between the GDA and CDA using CoAP.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL:  [https://github.com/Abbas-Rizvi/iot-python-components/](https://github.com/Abbas-Rizvi/iot-python-components/tree/labmodule09)

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/82bb2bf1-62be-4edb-917e-b0d6e1dcc0a4)

### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.


### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- CoapClientConnectorTest

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/f0ae352c-95bc-49ac-8d23-0e843571fab9)



EOF.
