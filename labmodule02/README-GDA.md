# Gateway Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-GDA-* issues (requirements) listed at [PIOT-INF-02-001 - Lab Module 02](https://github.com/orgs/programming-the-iot/projects/1#column-9974938).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

The implementation of the gateway device application is responisble for collecting system preformance analytics. It collects data such as 
CPU utilization, memory utilization, and disk utilization.

How does your implementation work?

The system perfomance manager collects performance analytics. The modules systemCpuUtilTask collects performance data on the cpu utilization, whereas 
the systemMemUtilTask collects performance data on the memory utilization. 

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/Abbas-Rizvi/iot-java-components

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/7017faf0-f736-49c8-97b5-53c87a3ec9a0)

### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest

  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/e3dcf958-9a60-4325-9d41-adf2c4259532)
  
- SystemMemUtilTest

  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/b1c6cff1-7dac-45d2-a891-978d9da4cc4a)

  
- SystemCpuUtilTaskTest

  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/78afd938-eb50-425b-a810-74ee379955fe)

  

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest

  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/681b3d07-eba7-4562-b363-ddb155d301fe)

  
- GatewayDeviceAppTest
  
  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/cb03f72e-38a4-4583-b16a-df986181eef9)

EOF.
