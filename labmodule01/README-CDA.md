# Constrained Device Application (Connected Devices)

## Lab Module 01

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-01-001 - Lab Module 01](https://github.com/orgs/programming-the-iot/projects/1#column-9974937).

### Description


NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

This module is focused on the initialization of the development environment. Specifically for the Constranied device
application for pydev and unit testing to test the validity of the environment set up prior to the run.

How does your implementation work?

The implementation works with the repository installed locally on each members device. Then with the installation of a 
python interpreter in eclipse IDE test cases were executed. Using the shared repository forked from programmingtheiot/book-
exercise-docs the code was altered and pushed to share with members of the group.

### Code Repository and Branch

![image](./image/repo.png)
![image](./image/branch.png)

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/Abbas-Rizvi/iot-python-components

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/4997ee1d-2df6-4af2-aa7c-e9269624bc19)

### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

ConfigUtilTest:
![image](./image/ConfigUnitTest.png)

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

ConstrainedDeviceAppTest:
![image](./image/ConstrainedDeviceAppTest.png)

EOF.
