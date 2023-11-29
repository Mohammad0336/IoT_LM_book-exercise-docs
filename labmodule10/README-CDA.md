# Constrained Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-10-001 - Lab Module 10](https://github.com/orgs/programming-the-iot/projects/1#column-10488510).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

How does your implementation work?

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: 

### UML Design Diagram(s)

NOTE: Include one or more UML designs representing your solution. It's expected each
diagram you provide will look similar to, but not the same as, its counterpart in the
book [Programming the IoT](https://learning.oreilly.com/library/view/programming-the-internet/9781492081401/).


### Unit Tests Executed

NOTE: TA's will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- N/A

### Integration Tests Executed

NOTE: TA's will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- PIOT-INT-10-001

``` 
<terminated> MqttClientPerformanceTest.py [/home/mohammad/programmingthelot/.venv/bin/python]
2023-11-29 10:15:42,896: ConfigUtil: INFO: Loading config: /home/mohammad/programmingtheiot/python-components/config/PiotConfig.props 2023-11-29 10:15:42,897: ConfigUtil: DEBUG:Config: ['Mqtt.GatewayService', 'Coap. GatewayService', 'ConstrainedDevice']
2023-11-29 10:15:42,897: ConfigUtil:INFO:Created instance of ConfigUtil: <programmingtheiot.common.ConfigUtil.ConfigUtil object at 0x7f389c1801d0> 2023-11-29 10:15:42,897:MqttClientConnector: INFO: MQTT Client ID: CDAMqttClientPerformanceTest001
2023-11-29 10:15:42,898: MqttClientConnector: INFO: 2023-11-29 10:15:42,898: MqttClientConnector: INFO: 2023-11-29 10:15:42,898: MqttClientConnector: INFO:
MQTT Broker Host: 127.0.0.1 MQTT Broker Port: 1883 MQTT Keep Alive: 60
MQTT Client ID:
CDAMqttClientPerformanceTest001
2023-11-29 10:15:42,898: MqttClientConnector: INFO: MQTT client connecting to broker at host: 127.0.0.1 2023-11-29 10:15:42,902:MqttClientConnector: INFO:Disconnecting MQTT client from broker: 127.0.0.1 2023-11-29 10:15:43,905:MqttClientPerformanceTest: INFO: Connect and Disconnect: 1008.503043 ms .2023-11-29 10:15:43,906: MqttClientConnector: INFO: 2023-11-29 10:15:43,906: MqttClientConnector: INFO: 2023-11-29 10:15:43,906: MqttClientConnector: INFO: 2023-11-29 10:15:43,906: MqttClientConnector: INFO:
MQTT Broker Host: 127.0.0.1 MQTT Broker Port: 1883 MQTT Keep Alive: 60
2023-11-29 10:15:43,906: MqttClientConnector: INFO: MQTT client connecting to broker at host: 127.0.0.1 2023-11-29 10:15:43,907:DataUtil: INFO:Created DataUtil instance.
2023-11-29 10:15:46,940:MqttClientConnector: INFO: Disconnecting MQTT client from broker: 127.0.0.1
2023-11-29 10:15:47,942:MqttClientPerformanceTest:INFO:
Testing Publish: QoS = 0 | msgs = 10000 | payload size = 264 | start = 1701125229721883.0 | end = 1701125232755647.5 | elapsed = 3.033764502 .2023-11-29 10:15:47,943:MqttClientConnector: INFO: MQTT Client ID: CDAMqttClientPerformanceTest001
2023-11-29 10:15:47,943: MqttClientConnector: INFO: 2023-11-29 10:15:47,943:MqttClientConnector: INFO:
2023-11-29 10:15:47,943: MqttClientConnector: INFO:
MQTT Broker Host: 127.0.0.1
MQTT Broker Port: 1883 MQTT Keep Alive: 60
2023-11-29 10:15:47,943: MqttClientConnector: INFO: MQTT client connecting to broker at host: 127.0.0.1
2023-11-29 10:15:47,944:DataUtil:INFO:Created DataUtil instance.
2023-11-29 10:15:52,326: MqttClientConnector: INFO: Disconnecting MQTT client from broker: 127.0.0.1 2023-11-29 10:15:53,328: MqttClientPerformanceTest:INFO:
Testing Publish: QoS = 1 | msgs = 10000 | payload size = 264 | start = 1701125233759100.0 | end = 1701125238139843.0 | elapsed = 4.379942972 2023-11-29 10:15:53,328:MqttClientConnector: INFO: MQTT Client ID: CDAMqttClientPerformanceTest001 2023-11-29 10:15:53,329: MqttClientConnector: INFO: 2023-11-29 10:15:53,329:MqttClientConnector: INFO:
2023-11-29 10:15:53,329: MqttClientConnector: INFO:
MQTT Broker Host: 127.0.0.1
MQTT Broker Port: 1883 MQTT Keep Alive: 60
2023-11-29 10:15:53,329: MqttClientConnector: INFO: MQTT client connecting to broker at host: 127.0.0.1 2023-11-29 10:15:53,330:DataUtil:INFO:Created DataUtil instance.
2023-11-29 10:15:58,356: MqttClientConnector: INFO: Disconnecting MQTT client from broker: 127.0.0.1
2023-11-29 10:15:59,358: MqttClientPerformanceTest: INFO:
Testing Publish: QoS = 2 | msgs = 10000 | payload size = 264 | start = 1701125239141879.8 | end = 1701125245167484.0 | elapsed = 6.0256843319999995
Ran 4 tests in 17.460s
OK
```

- PIOT-CDA-10-001

- PIOT-CDA-10-002

- PIOT-CDA-10-003

- PIOT-CDA-10-004

- PIOT-INT-10-003

- PIOT-INT-10-004

EOF.
