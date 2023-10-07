# Constrained Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-05-001 - Lab Module 05](https://github.com/orgs/programming-the-iot/projects/1#column-10488421).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

This implementation works through providing data storage for the various system performance classes.
It also allows for conversion to and from json for each of the data points.

How does your implementation work?

The task includes updating method signatures within the class, implementing methods for converting between various data objects and JSON, and ensuring import statements are correctly placed. The provided code demonstrates how to convert objects like ActuatorData to JSON and vice versa using the built-in json library and a custom JsonDataEncoder class. The code also provides instructions for handling similar conversions for other data types like SensorData and SystemPerformanceData.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/tree/default

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/73917749/af46fc67-af7a-49fe-a5c0-2e1416c7b79c)


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/73917749/9124b839-c0e6-4d2c-88a5-bd0d26e53c2a)
![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/73917749/f1727adf-1e81-47a0-8b88-d15ac039ffda)


### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

N/A

EOF.
