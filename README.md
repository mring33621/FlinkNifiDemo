# FlinkNifiDemo
Setup instructions for my recent Flink-NiFi demo.

[Refer to the Demo Slides](http://www.slideshare.net/mring33/flink-and-nifi-two-stars-in-the-apache-big-data-constellation)

1. Install [Java 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
2. Install a [NATS Messaging server](http://nats.io/download/)
3. Install [Apache NiFi] (https://nifi.apache.org/download.html)
4. Clone and install the following Maven projects:
  * https://github.com/mring33621/scripting-for-nifi
  * https://github.com/mring33621/nats-messaging-for-nifi
  * https://github.com/mring33621/nats-messaging-for-flink
  * https://github.com/mring33621/MarketData
  * https://github.com/mring33621/StockMarketTicker
  * https://github.com/mring33621/StreamVisServer
  * https://github.com/mring33621/DemoFlinkEngines
5. Copy the following .nar files into NiFi/lib
  * nifi-scripting-nar-x.y.z.nar
  * nifi-nats-nar-x.y.z.nar
6. Run the gnatsd server
7. Run NiFi then import the FlinkNifiDemoFlow.xml file
8. Unzip var.zip into your /var dir
9. Run DemoFlinkEngines com.mattring.demoflinkengines.EnginesMain
10. Run StreamVisServer com.mattring.streamvisserver.ServerMain
11. Point your browser to http://localhost:4567/DemoPages/dashboard.html to watch the fun
