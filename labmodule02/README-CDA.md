# Constrained Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-02-001 - Lab Module 02](https://github.com/orgs/programming-the-iot/projects/1#column-9974938).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

This module utilizes the architechure from module one and implements monitoring for performance in the cda.
Regular system logs are displayed to show the progress of implementation.

How does your implementation work?

The text informs to implement modules that monitor specific performance data characteristics. For example, 
the SystemPerformanceManager module monitors system performance data. More specifically 
it collects data through the System CpuUtilTask and MemUtilTask modules.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/Abbas-Rizvi/iot-python-components

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/2daaaf3c-6ff1-462c-8f73-0ba8455b370d)

### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/07654e9b-9d2e-4667-9dcd-71d28c12fa24)
  
- SystemCpuUtilTaskTest
  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/ad11d351-0167-4c9f-b738-65910bf81dd2)

- SystemMemUtilTaskTest

  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/84eb82e4-3f08-41da-bb8b-5fcd49510199)

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- ConstrainedDeviceAppTest
  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/c3c8c529-88cb-4bfe-a0be-167287fe8056)
  
- SystemPerformanceManagerTest
  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/b5710195-dccf-4fde-ad62-e3b1f1970fc3)

EOF.
