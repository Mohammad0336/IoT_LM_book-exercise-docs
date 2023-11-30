# Constrained Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-CDA-* issues (requirements) listed at [PIOT-INF-10-001 - Lab Module 10](https://github.com/orgs/programming-the-iot/projects/1#column-10488510).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

The implementation uses Edge Tier applications for CDA and GDA in an IoT environment via CoAP and MQTT. Emphasis is on 
security with TLS encryption for MQTT communication, securing message exchange. It configures Mosquitto broker for TLS, modifies 
MqttClientConnector class for encrypted connections, and addresses credential management. Overall, it establishes a secure 
communication framework in the IoT Edge Tier.

How does your implementation work?

The implementation uses Edge Tier applications for CDA and GDA in an IoT environment via CoAP and MQTT, with a focus on TLS 
encryption for MQTT connections. This involves configuring Mosquitto broker for TLS, secure loading of credentials, and modifying 
MqttClientConnector class in both applications. The modifications include SSL socket factory initialization and configuring MQTT 
client connection for encryption.

### Code Repository and Branch

NOTE: Be sure to include the branch (e.g. https://github.com/programming-the-iot/python-components/tree/alpha001).

URL: https://github.com/Abbas-Rizvi/iot-python-components

### UML Design Diagram(s)

![image](https://github.com/Mohammad0336/IoT_LM_book-exercise-docs/assets/81828400/8eca9e0f-4a75-427b-aa0f-90752918d32b)

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

```
<terminated> MqttClientConnectorTest.py [unittest] [/home/mohammad/programmingtheiot/.venv/bin/python] 0.00s Debugger warning: It seems that frozen modules are being used, which may
0.00s make the debugger miss breakpoints. Please pass -Xfrozen_modules-off
0.00s
to python to disable frozen modules.
0.00s - Note: Debugging will proceed. Set PYDEVD_DISABLE_FILE_VALIDATION=1 to disable this validation.
Finding files... done.
Importing test modules ... done.
2023-11-29 10:15:42,896:MqttClientConnectorTest: INFO: Testing MqttClientConnector class...
2023-11-29 10:15:42,898: ConfigUtil: INFO: Loading config: /home/mohammad/programmingtheiot/python-components/config/PiotConfig.props
2023-11-29 10:15:42,900: ConfigUtil: DEBUG:Config: ['Mqtt.GatewayService', 'Coap. GatewayService', 'ConstrainedDevice']
2023-11-29 10:15:42,901: ConfigUtil: INFO: Created instance of ConfigUtil: <programmingtheiot.common.ConfigUtil.ConfigUtil object at 0x7f763aa09a10> 2023-11-29 10:15:42,901: MqttClientConnector: INFO: MQTT Client ID: MqttclientTest
2023-11-29 10:15:42,901: MqttClientConnector: INFO: 2023-11-29 10:15:42,901: MqttClientConnector: INFO:
2023-11-29 10:15:42,901: MqttClientConnector: INFO:
MQTT Broker Host: 127.0.0.1
MQTT Broker Port: 1883 MQTT Keep Alive: 60
2023-11-29 10:15:42,902:MqttClientConnector: INFO: MQTT client connecting to broker at host: 127.0.0.1 2023-11-29 10:15:47,905: MqttClientConnector: INFO:Disconnecting MQTT client from broker: 127.0.0.1
Ran 8 tests in 65.050s
OK (skipped=7)
```

- PIOT-CDA-10-002

```
<terminated> DeviceDataManagerCallbackTest.py [/home/mohammad/programmingtheiot/.venv/bin/python]
2023-11-29 11:25:15,526: DeviceDataManagerCallbackTest: INFO: Testing DeviceDataManager class...
2023-11-29 11:25:15,526: ConfigUtil: INFO: Loading config: /home/mohammad/programmingtheiot/python-components/config/PiotConfig.props 2023-11-29 11:25:15,527: ConfigUtil: DEBUG:Config: ['Mqtt. GatewayService', 'Coap. GatewayService', 'ConstrainedDevice']
2023-11-29 11:25:15,527: ConfigUtil: INFO:Created instance of ConfigUtil: <programmingtheiot.common.ConfigUtil.ConfigUtil object at 0x7f0ae1188b10> 2023-11-29 11:25:15,527:MqttClientConnector: INFO: MQTT Client ID: DeviceDataMQTT
2023-11-29 11:25:15,527:MqttClientConnector: INFO: 2023-11-29 11:25:15,527:MqttClientConnector: INFO: 2023-11-29 11:25:15,527:MqttClientConnector: INFO:
MQTT Broker Host: 127.0.0.1 MQTT Broker Port: 1883
MQTT Keep Alive: 60
2023-11-29 11:25:15,527: DeviceDataManager: INFO: Starting DeviceDataManager...
2023-11-29 11:25:15,527: MqttClientConnector: INFO: MQTT client connecting to broker at host: 127.0.0.1
2023-11-29 11:25:15,532: DeviceDataManager: INFO:Started DeviceDataManager.
2023-11-29 11:25:15,534: MqttClientConnector: INFO: [Callback] Connected to MQTT broker. Result code: 0
2023-11-29 11:25:15,535:MqttClientConnector: INFO: MQTT client subscribed: <paho.mqtt.client.Client object at 0x7f0ae0b66110> 2023-11-29 11:25:15,536:MqttClientConnector: INFO: MQTT client subscribed: <paho.mqtt.client.Client object at 0x7f0ae0b66110>
2023-11-29 11:25:25,533: DeviceDataManager: INFO:Stopping DeviceDataManager...
2023-11-29 11:25:25,534: MqttClientConnector: INFO: Disconnecting MQTT client from broker: 127.0.0.1 2023-11-29 11:25:25,534: DeviceDataManager: INFO: Stopped DeviceDataManager.
Ran 1 test in 10.010s
OK
```

- PIOT-CDA-10-003

```
<terminated> MqttClientConnectorTest.py [/home/mohammad/programmingthelot/.venv/bin/python]
2023-11-29 11:35:40,874:MqttClientConnectorTest: INFO: Testing MqttClientConnector class...
2023-11-29 11:35:40,874: ConfigUtil: INFO: Loading config: /home/mohammad/programmingtheiot/python-components/config/PiotConfig.props 2023-11-29 11:35:40,874: ConfigUtil: DEBUG:Config: ['Mqtt. GatewayService', 'Coap. GatewayService', 'ConstrainedDevice']
2023-11-29 11:35:40,875: ConfigUtil: INFO:Created instance of ConfigUtil: <programmingtheiot.common.ConfigUtil.ConfigUtil object at 0x7f1e18981490> 2023-11-29 11:35:40,875: MqttClientConnector: INFO: MQTT Client ID: MqttclientTest 2023-11-29 11:35:40,875: MqttClientConnector: INFO: 2023-11-29 11:35:40,875: MqttClientConnector: INFO:
2023-11-29 11:35:40,875: MqttClientConnector: INFO:
MQTT Broker Host: 127.0.0.1
MQTT Broker Port: 1883
MQTT Keep Alive: 60
ssssss2023-11-29 11:35:40,876: DataUtil: INFO:Created DataUtil instance.
2023-11-29 11:35:40,876: MqttClientConnector: INFO: MQTT client connecting to broker at host: 127.0.0.1
2023-11-29 11:35:40,882: MqttClientConnector: INFO: [Callback] Connected to MQTT broker. Result code: 0
2023-11-29 11:35:40,886: MqttClientConnector: INFO: MQTT client subscribed: <paho.mqtt.client.Client object at 0x7f1e18969450>
2023-11-29 11:35:45,886: MqttClientConnector: INFO: [Callback] Actuator command message received. Topic: PIOT/ConstrainedDevice/ActuatorCmd. 2023-11-29 11:35:45,886: DataUtil: INFO:Created DataUtil instance.
2023-11-29 11:35:45,886: DefaultDataMessageListener: INFO: Actuator Command Msg:
2023-11-29 11:36:45,886: MqttClientConnector: INFO: Disconnecting MQTT client from broker: 127.0.0.1
.S
Ran 8 tests in 65.043s
OK (skipped=7)
```

- PIOT-CDA-10-004

```
<terminated> DeviceDataManagerIntegrationTest.py [/home/mohammad/programmingthelot/.venv/bin/python] 2023-11-29 11:50:22,133: DeviceDataManagerIntegrationTest: INFO: Testing DeviceDataManager class...
2023-11-29 11:50:22,136: ConfigUtil: INFO: Loading config: /home/mohammad/programming theiot/python-components/config/PiotConfig.props 2023-11-29 11:50:22,137: ConfigUtil: DEBUG:Config: ['Mqtt. GatewayService', 'Coap. GatewayService', 'ConstrainedDevice'] 2023-11-29 11:50:22,137: ConfigUtil: INFO: Created instance of ConfigUtil: 2023-11-29 11:50:22,140: MqttClientConnector: INFO: 2023-11-29 11:50:22,140: MqttClientConnector: INFO:
2023-11-29 11:50:22,140: MqttClientConnector: INFO: 2023-11-29 11:50:22,140: MqttClientConnector: INFO:
<programmingtheiot.common.ConfigUtil.ConfigUtil object at 0x7f66dbbf67d0>
MQTT Client ID: DeviceDataMQTT MQTT Broker Host: 127.0.0.1 MQTT Broker Port: 1883
MQTT Keep Alive: 60
2023-11-29 11:50:22,140: DeviceDataManager: INFO: Starting DeviceDataManager...
2023-11-29 11:50:22,141: MqttClientConnector: INFO:MQTT client connecting to broker at host: 127.0.0.1 2023-11-29 11:50:22,157:MqttClientConnector: INFO: [Callback] Connected to MQTT broker. Result code: 0
2023-11-29 11:50:22,161: MqttClientConnector: INFO: MQTT client subscribed: <paho.mqtt.client.Client object at 0x7f66dbb06fd0> 2023-11-29 11:50:22,164: DeviceDataManager: INFO:Started DeviceDataManager.
2023-11-29 11:50:22,165: MqttClientConnector: INFO: MQTT client subscribed: <paho.mqtt.client.Client object at 0x7f66dbb06fd0> 2023-11-29 11:50:37,164: DeviceDataManager: INFO: Stopping DeviceDataManager...
2023-11-29 11:50:37,165: MqttClientConnector: INFO: Disconnecting MQTT client from broker: 127.0.0.1 2023-11-29 11:50:37,168: DeviceDataManager: INFO: Stopped DeviceDataManager.
Ran 1 test in 15.036s
OK
```

- PIOT-INT-10-003

```
<terminated> DeviceDataManagerIntegrationTest.py [/home/mohammad/programmingthelot/.venv/bin/python] 2023-11-29 12:05:10,255: DeviceDataManagerIntegrationTest: INFO: Testing DeviceDataManager class...
2023-11-29 12:05:10,255: ConfigUtil: INFO: Loading config: /home/mohammad/programming theiot/python-components/config/PiotConfig.props 2023-11-29 12:05:10,255: ConfigUtil: DEBUG:Config: ['Mqtt. GatewayService', 'Coap. GatewayService', 'ConstrainedDevice']
2023-11-29 12:05:10,255: ConfigUtil: INFO:Created instance of ConfigUtil: <programming theiot.common.ConfigUtil.ConfigUtil object at 0x7f5db2343b90> 2023-11-29 12:05:10,255:MqttClientConnector: INFO: MQTT Client ID: DeviceDataMQTT
2023-11-29 12:05:10,256:MqttClientConnector: INFO: 2023-11-29 12:05:10,256:MqttClientConnector: INFO: 2023-11-29 12:05:10,256:MqttClientConnector: INFO:
MQTT Broker Host: 127.0.0.1
MQTT Broker Port: 1883 MQTT Keep Alive: 60
2023-11-29 12:05:10,256: DeviceDataManager: INFO:Starting DeviceDataManager...
2023-11-29 12:05:10,256:MqttClientConnector: INFO: MQTT client connecting to broker at host: 127.0.0.1 2023-11-29 12:05:10,262: DeviceDataManager: INFO:Started DeviceDataManager.
2023-11-29 12:05:10,262:MqttClientConnector: INFO: [Callback] Connected to MQTT broker. Result code:
2023-11-29 12:05:10,264:MqttClientConnector: INFO: MQTT client subscribed: <paho.mqtt.client.Client object at 0x7f5db29ee9d0> 2023-11-29 12:05:10,264:MqttClientConnector: INFO: MQTT client subscribed: <paho.mqtt.client.Client object at 0x7f5db29ee9d0> 2023-11-29 12:06:50,262: DeviceDataManager: INFO: Stopping DeviceDataManager...
2023-11-29 12:06:50,263: MqttClientConnector: INFO: Disconnecting MQTT client from broker: 127.0.0.1 2023-11-29 12:06:50,263: DeviceDataManager: INFO: Stopped DeviceDataManager.
Ran 1 test in 100.009s
OK
```

- PIOT-INT-10-004

```
<terminated> DeviceDataManagerIntegrationTest.py [/home/mohammad/programmingthelot/.venv/bin/python] 2023-11-29 12:15:32,497: DeviceDataManagerIntegrationTest: INFO: Testing DeviceDataManager class...
2023-11-29 12:15:32,497: ConfigUtil: INFO: Loading config: /home/mohammad/programming theiot/python-components/config/PiotConfig.props 2023-11-29 12:15:32,500: ConfigUtil: DEBUG:Config: ['Mqtt. GatewayService', 'Coap.GatewayService', 'ConstrainedDevice']
2023-11-29 12:15:32,500: ConfigUtil: INFO:Created instance of ConfigUtil: <programmingtheiot.common.ConfigUtil.ConfigUtil object at 0x7fd2fd87f190> 2023-11-29 12:15:32,500:MqttClientConnector: INFO: MQTT Client ID: DeviceDataMQTT
MQTT Broker Host: 127.0.0.1
MQTT Broker Port: 1883 MQTT Keep Alive: 60
2023-11-29 12:15:32,500:MqttClientConnector: INFO: 2023-11-29 12:15:32,500:MqttClientConnector: INFO: 2023-11-29 12:15:32,500:MqttClientConnector: INFO: 2023-11-29 12:15:32,500: DeviceDataManager: INFO:Starting DeviceDataManager...
2023-11-29 12:15:32,500:MqttClientConnector: INFO: Enabling TLS encryption...
/home/mohammad/programmingtheiot/.venv/lib/python3.11/site-packages/paho/mqtt/client.py:792: DeprecationWarning: ssl.PROTOCOL_TLSv1_2 is deprecated
context = ssl.SSLContext(tls_version)
2023-11-29 12:15:32,509: MqttClientConnector: INFO: MQTT client connecting to broker at host: 127.0.0.1
2023-11-29 12:15:32,522: DeviceDataManager: INFO: Started DeviceDataManager.
2023-11-29 12:15:32,529: MqttClientConnector: INFO: [Callback] Connected to MQTT broker. Result code: 0
2023-11-29 12:15:32,530:MqttClientConnector: INFO: MQTT client subscribed: <paho.mqtt.client.Client object at 0x7fd2fceacb90> 2023-11-29 12:15:32,530:MqttClientConnector: INFO: MQTT client subscribed: <paho.mqtt.client.Client object at 0x7fd2fceacb90> 2023-11-29 12:17:12,525: DeviceDataManager: INFO: Stopping DeviceDataManager...
2023-11-29 12:17:12,525: MqttClientConnector: INFO:Disconnecting MQTT client from broker: 127.0.0.1 2023-11-29 12:17:12,525: DeviceDataManager: INFO:Stopped DeviceDataManager.
Ran 1 test in 100.028s
OK
```

EOF.
