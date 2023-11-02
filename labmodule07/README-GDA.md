# Gateway Device Application (Connected Devices)

## Lab Module 07

Be sure to implement all the PIOT-GDA-* issues (requirements) listed at [PIOT-INF-07-001 - Lab Module 07](https://github.com/orgs/programming-the-iot/projects/1#column-10488499).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

The implementation involves implementing a Java class 'MqttClientConnector' that serves as a module to interact with an MQTT broker. This class has been stubbed out, providing a foundation to build the MQTT client pub/sub
functionality. The primary objective of this implementation is to add and configure callbacks within the module to handle MQTT client events, specifically for connection (connect and disconnect) and 
message received events. These callbacks are essential for managing the MQTT client's connection state and handling incoming messages from subbed topics.

How does your implementation work?

The MqttClientConnector class is equipped with methods for connecting to and disconnecting from MQTT brokers, publishing messages, and subscribing to topics. It uses callbacks to respond to connection events, like 
successful connections and disconnections, as well as incoming messages on subscribed topics. This design enables it to support pub/sub functionality for versatile use in IoT use cases and allows smooth 
interactions with MQTT brokers while playing a important role in integrating MQTT communication capabilities into DeviceDataManager.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/Abbas-Rizvi/iot-java-components

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- refer to labmodule06 unit tests
- 
- 

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- PIOT-GDA-07-001:
  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/662c4b8c-54ea-42e4-9d73-54ec3c8221a4)
- PIOT-GDA-07-002:
  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/f1107bfc-57da-401b-abe8-603dc859a8dd)
- PIOT-GDA-07-003:
  ![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/20b879ff-2dd3-4b01-97e3-86750387931d)

EOF.
