# Cab Booking location sharing using Apache Kafka & Spring Boot
 Simple illustration of streaming of live location sharing by driver i.e producer in the form of latitude & longitude & receiving it by user i.e consumer using Apache Kafka & Spring Boot

***

#### Steps to start Kafka server (for Windows):

 1. Download Apache kafka
 2. Go inside kafka folder
 3. Start zookeeper server
  Run on cmd `.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties`
 4. Start Kafka server
    On new cmd `.\bin\windows\kafka-server-start.bat .\config\server.properties`
 5. Create a topic to store events on kafka server
    On new cmd `\bin\windows>kafka-topics.bat --create --bootstrap-server localhost:9092 --topic test`
 6. To see the topic/describe the topic
    `\bin\windows>kafka-topics.bat --describe --bootstrap-server localhost:9092 --topic test`
 7. Start the producer
    On new cmd `\bin\windows>kafka-console-producer.bat --topic test --bootstrap-server localhost:9092`
 8. Start the consumer
    On new cmd `\bin\windows>kafka-console-consumer.bat --topic test --bootstrap-server localhost:9092 --from-beginning`

 - Note: Don't close any of the cmd commands


***

### Screenshots

- Receiving data (latitude & longitude) by consumer on CLI

![receiving data on CLI consumer](https://github.com/abhishekgupta44/kafka-cab-booking/assets/82182042/688a0025-a5a4-45b7-a533-c7bff32d9348)

- Receiving data (latitude & longitude) by consumer on IDE

![receiving data on IDE consumer](https://github.com/abhishekgupta44/kafka-cab-booking/assets/82182042/d83773c3-8cd4-4d18-9d3a-677bab7d1e95)


  
