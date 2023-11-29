# Gateway Device Application (Connected Devices)

## Lab Module 10

Be sure to implement all the PIOT-GDA-* issues (requirements) listed at [PIOT-INF-10-001 - Lab Module 10](https://github.com/orgs/programming-the-iot/projects/1#column-10488510).

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

- testConnectAndDisconnect()

```
<terminated> MqttClientPerformance Test [JUnit] /usr/lib/jvm/java-17-openjdk-amd64/bin/java (Nov 29, 2023, 12:30:45 PM-12:30:47 PM) [pid: 4240] Nov 29, 2023 12:30:47 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters
INFO: Checking if credentials file exists and is loadable...
Nov 29, 2023 12:30:47 PM programmingtheiot.common.ConfigUtil getCredentials
WARNING: Credential file non-existent: ./cred/PiotMqttCred.props. Ignoring.
Nov 29, 2023 12:30:47 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters WARNING: No credentials are set.
Nov 29, 2023 12:30:47 PM programmingtheiot.gda.connection.MqttClientConnector initClientParameters
INFO: Using URL for broker conn: tcp://127.0.0.1:1883
Nov 29, 2023 12:30:47 PM programmingtheiot.gda.connection.MqttClientConnector connectClient
INFO: MQTT client connecting to broker: tcp://127.0.0.1:1883
Nov 29, 2023 12:30:47 PM programmingtheiot.gda.connection.MqttClientConnector connectComplete
INFO: connectComplete method called. Client has successfully connected.
Nov 29, 2023 12:30:47 PM programmingtheiot.gda.connection.MqttClientConnector disconnectClient
INFO: Disconnecting MQTT client from broker: tcp://127.0.0.1:1883
Nov 29, 2023 12:30:47 PM programmingtheiot.part03.integration.connection.MqttClient PerformanceTest testConnectAndDisconnect INFO: Connect and Disconnect [1]: 451 ms
```

- testPublishQoS0()

```
<terminated> MqttClientPerformanceTest [JUnit] /usr/lib/jvm/java-17-openjdk-amd64/bin/java (Nov 29, 2023, 12:32:36 PM–12:32:38 PM) [pid: 4315] Nov 29, 2023 12:32:38 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters
INFO: Checking if credentials file exists and is loadable...
Nov 29, 2023 12:32:38 PM programmingtheiot.common.ConfigUtil getCredentials
WARNING: Credential file non-existent: ./cred/PiotMqttCred.props. Ignoring.
Nov 29, 2023 12:32:38 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters WARNING: No credentials are set.
Nov 29, 2023 12:32:38 PM programmingtheiot.gda.connection.MqttClientConnector initClientParameters
INFO: Using URL for broker conn: tcp://127.0.0.1:1883
Nov 29, 2023 12:32:38 PM programmingtheiot.gda.connection.MqttClientConnector connectClient
INFO: MQTT client connecting to broker: tcp://127.0.0.1:1883
Nov 29, 2023 12:32:38 PM programmingtheiot.gda.connection.MqttClientConnector connectComplete
INFO: connectComplete method called. Client has successfully connected.
Nov 29, 2023 12:32:38 PM programmingtheiot.gda.connection.MqttClientConnector disconnectClient
INFO: Disconnecting MQTT client from broker: tcp://127.0.0.1:1883
Nov 29, 2023 12:32:38 PM programmingtheiot.part03.integration.connection.MqttClientPerformanceTest execTestPublish
INFO: \n\tTesting Publish: QoS = 0 | msgs = 10000 | payload size = 212 | start = 1.70112448E9 | end = 1.70112448E9 | elapsed = 9.16
```

- testPublishQoS1()

```
<terminated> MqttClientPerformance Test [JUnit] /usr/lib/jvm/java-17-openjdk-amd64/bin/java (Nov 29, 2023, 12:33:50 PM–12:34:13 PM) [pid: 4391] Nov 29, 2023 12:34:04 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters INFO: Checking if credentials file exists and is loadable...
Nov 29, 2023 12:34:04 PM programmingtheiot.common.ConfigUtil getCredentials
WARNING: Credential file non-existent: ./cred/PiotMqttCred.props. Ignoring.
Nov 29, 2023 12:34:04 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters WARNING: No credentials are set.
Nov 29, 2023 12:34:04 PM programmingtheiot.gda.connection.MqttClientConnector initClientParameters
INFO: Using URL for broker conn: tcp://127.0.0.1:1883
Nov 29, 2023 12:34:04 PM programmingtheiot.gda.connection.MqttClientConnector connectClient
INFO: MQTT client connecting to broker: tcp://127.0.0.1:1883
Nov 29, 2023 12:34:04 PM programmingtheiot.gda.connection.MqttClientConnector connectComplete
INFO: connectComplete method called. Client has successfully connected.
Nov 29, 2023 12:34:13 PM programmingtheiot.gda.connection.MqttClientConnector disconnectClient
INFO: Disconnecting MQTT client from broker: tcp://127.0.0.1:1883
Nov 29, 2023 12:34:13 PM programmingtheiot.part03.integration.connection.MqttClientPerformanceTest execTestPublish
INFO: \n\tTesting Publish: QoS = 1 | msgs = 10000 | payload size = 212 | start = 1.70112461E9 | end = 1.70112461E9 | elapsed = 17.751
```

- testPublishQoS2()

```
<terminated> MqttClientPerformance Test [JUnit] /usr/lib/jvm/java-17-openjdk-amd64/bin/java (Nov 29, 2023, 12:40:22 PM–12:40:59 PM) [pid: 4454] Nov 29, 2023 12:40:24 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters INFO: Checking if credentials file exists and is loadable...
Nov 29, 2023 12:40:24 PM programmingtheiot.common.ConfigUtil getCredentials
WARNING: Credential file non-existent: ./cred/PiotMqttCred.props. Ignoring.
Nov 29, 2023 12:40:24 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters WARNING: No credentials are set.
Nov 29, 2023 12:40:24 PM programmingtheiot.gda.connection.MqttClientConnector initClientParameters
INFO: Using URL for broker conn: tcp://127.0.0.1:1883
Nov 29, 2023 12:40:24 PM programmingtheiot.gda.connection.MqttClientConnector connectClient
INFO: MQTT client connecting to broker: tcp://127.0.0.1:1883
Nov 29, 2023 12:40:24 PM programmingtheiot.gda.connection.MqttClientConnector connectComplete
INFO: connectComplete method called. Client has successfully connected.
Nov 29, 2023 12:40:59 PM programmingtheiot.gda.connection.MqttClientConnector disconnectClient
INFO: Disconnecting MQTT client from broker: tcp://127.0.0.1:1883
Nov 29, 2023 12:40:59 PM programmingtheiot.part03.integration.connection.MqttClientPerformanceTest execTestPublish
INFO: \n\tTesting Publish: QoS 2 | msgs = 10000 | payload size = 212 | start = 1.70112461E9 | end = 1.70112461E9 | elapsed = 34.452
```

- PIOT-GDA-10-001

```
<terminated> MqttClientConnectorTest [JUnit] /usr/lib/jvm/java-17-openjdk-amd64/bin/java (Nov 29, 2023, 2:18:42 PM–2:19:48 PM) [pid: 7190] Nov 29, 2023 2:18:42 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters
INFO: Checking if credentials file exists and is loadable...
Nov 29, 2023 2:18:42 PM programmingtheiot.common.ConfigUtil getCredentials
WARNING: Credential file non-existent: ./cred/PiotMqttCred.props. Ignoring.
Nov 29, 2023 2:18:42 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters WARNING: No credentials are set.
Nov 29, 2023 2:18:42 PM programmingtheiot.gda.connection.MqttClientConnector initClientParameters
INFO: Using URL for broker conn: tcp://127.0.0.1:1883
Nov 29, 2023 2:18:42 PM programmingtheiot.gda.connection.MqttClientConnector connectClient
INFO: MQTT client connecting to broker: tcp://127.0.0.1:1883
Nov 29, 2023 2:18:43 PM programmingtheiot.gda.connection.MqttClientConnector connectComplete
INFO: connectComplete method called. Client has successfully connected.
Nov 29, 2023 2:18:43 PM programmingtheiot.gda.connection.MqttClientConnector connectClient WARNING: MQTT client already connected to broker: tcp://127.0.0.1:1883
Nov 29, 2023 2:19:48 PM programmingtheiot.gda.connection.MqttClientConnector disconnectClient INFO: Disconnecting MQTT client from broker: tcp://127.0.0.1:1883
Nov 29, 2023 2:19:48 PM programmingtheiot.gda.connection.MqttClientConnector disconnectClient WARNING: MQTT client not connected to broker: tcp://127.0.0.1:1883
```

- PIOT-GDA-10-002
- testConnectAndDisconnect()

```
<terminated> MqttClientConnector Test [Junit] /usr/lib/jvm/java-17-openjdk-amd64/bin/java (Nov 29, 2023, 2:10:15 PM–2:11:21 PM) [pld: 7500] INFO: MQTT client connecting to broker: tcp://127.0.0.1:1883
Nov 29, 2023 2:10:16 PM programmingtheiot.gda.connection.MqttClientConnector connectClient SEVERE: Failed to connect MQTT client to broker: tcp://127.0.0.1:1883
Connect already in progress (32110)
at org.eclipse.paho.client.mqttv3.MqttAsyncClient.connect(MqttAsyncClient.java:602) at org.eclipse.paho.client.mqttv3.MqttAsyncClient.connect(MqttAsyncClient.java:584)
at programmingtheiot.gda.connection.MqttClientConnector.connectClient(MqttClientConnector.java:128)
at programmingtheiot.part03.
integration.connection.MqttClientConnectorTest.testConnectAndDisconnect (MqttClientConnectorTest.java:77)
at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77)
at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) at java.base/java.lang.reflect.Method.invoke(Method.java:568)
at
org.junit.runners.model. FrameworkMethod$1.runReflectiveCall(FrameworkMethod.java:59)
at org.junit.internal.runners.model.ReflectiveCallable.run(ReflectiveCallable.java:12)
at org.junit.runners.model. FrameworkMethod.invokeExplosively (FrameworkMethod.java:56)
at org.junit.internal.runners.statements. InvokeMethod.evaluate(InvokeMethod.java:17) at org.junit.internal.runners.statements. RunBefores.evaluate(RunBefores.java:26) at org.junit.internal.runners.statements. RunAfters.evaluate(RunAfters.java:27) at org.junit.runners. ParentRunner$3.evaluate(ParentRunner.java:306)
at org.junit.runners.BlockJUnit4Class Runner$1.evaluate(BlockJUnit4ClassRunner.java:100) at org.junit.runners. ParentRunner.runLeaf (ParentRunner.java:366)
at org.junit.runners.BlockJUnit4ClassRunner.runChild (BlockJUnit4ClassRunner.java:103) at org.junit.runners. BlockJUnit4ClassRunner.runChild (BlockJUnit4ClassRunner.java:63) at org.junit.runners. ParentRunner$4.run(ParentRunner.java:331)
at org.junit.runners. ParentRunner$1.schedule (ParentRunner.java:79) at org.junit.runners. ParentRunner.runChildren (ParentRunner.java:329) at org.junit.runners. ParentRunner.access$100(ParentRunner.java:66) at org.junit.runners. ParentRunner$2.evaluate(ParentRunner.java:293) at org.junit.runners.ParentRunner$3.evaluate(ParentRunner.java:306)
at org.junit.runners. ParentRunner.run(ParentRunner.java:413)
at org.eclipse.jdt.internal.junit4.runner.JUnit4TestReference.run(JUnit4TestReference.java:93) at org.eclipse.jdt.internal.junit.runner. TestExecution.run(TestExecution.java:40)
at org.eclipse.jdt.internal.junit.runner. RemoteTestRunner.runTests (RemoteTestRunner.java:529) at org.eclipse.jdt.internal.junit.runner. RemoteTestRunner.runTests (RemoteTestRunner.java:756) at org.eclipse.jdt.internal.junit.runner. RemoteTestRunner.run(RemoteTestRunner.java:452) at org.eclipse.jdt.internal.junit.runner. RemoteTestRunner.main(RemoteTestRunner.java:210)
Nov 29, 2023 2:10:17 PM programmingtheiot.gda.connection.MqttClientConnector connectComplete INFO: MQTT connection successful (is reconnect = false). Broker: tcp://127.0.0.1:1883
Nov 29, 2023 2:11:21 PM programmingtheiot.gda.connection.MqttClientConnector disconnectClient INFO: Disconnecting MQTT client from broker: tcp://127.0.0.1:1883
Nov 29, 2023 2:11:21 PM programmingtheiot.gda.connection.MqttClientConnector disconnectClient WARNING: MQTT client not connected to broker: tcp://127.0.0.1:1883
```

- testActuatorCommandResponseSubscription()

```
<terminated> MqttClientConnector Test [JUnit] /usr/lib/jvm/java-17-openjdk-amd64/bin/java (Nov 29, 2023, 1:45:30 PM–1:45:39 PM) [pid: 7650 Nov 29, 2023 1:45:34 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters INFO: Checking if credentials file exists and is loadable...
Nov 29, 2023 1:45:34 PM programmingtheiot.common.ConfigUtil getCredentials
WARNING: Credential file non-existent: ./cred/PiotMqttCred.props. Ignoring.
Nov 29, 2023 1:45:34 PM programmingtheiot.gda.connection.MqttClientConnector initCredentialConnectionParameters WARNING: No credentials are set.
Nov 29, 2023 1:45:34 PM programmingtheiot.gda.connection.MqttClientConnector initClientParameters
INFO: Using URL for broker conn: tcp://127.0.0.1:1883
Nov 29, 2023 1:45:34 PM programmingtheiot.gda.connection.MqttClientConnector connectClient
INFO: MQTT client connecting to broker: tcp://127.0.0.1:1883
Nov 29, 2023 1:45:35 PM programmingtheiot.gda.connection.MqttClientConnector connectComplete
INFO: MQTT connection successful (is reconnect = false). Broker: tcp://127.0.0.1:1883
Nov 29, 2023 1:45:37 PM programmingtheiot.gda.connection.MqttClientConnector messageArrived
INFO: messageArrived method called. A message has arrived
Nov 29, 2023 1:45:39 PM programmingtheiot.gda.connection.MqttClientConnector disconnectClient
INFO: Disconnecting MQTT client from broker: tcp://127.0.0.1:1883
```

- PIOT-GDA-10-003

- PIOT-INT-10-003

- PIOT-INT-10-004

- 

EOF.
