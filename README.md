# KafkaWithSpringBoot
This is sample project which consumes topics/queues/procedures. This application deserializes messages into JSON object. 

Apache Kafka stores and transports Byte arrays in its topics. It ships with a number of built in (de)serializers but a JSON one is not included. Luckily, the Spring Kafka framework includes a support package that contains a JSON (de)serializer that uses a Jackson ObjectMapper under the covers.


This sample application shows how to use basic Spring Boot configuration to set up a producer to a topic with multiple partitions and a consumer group with three different consumers.

[![Kafka Configuration Example](img/kafka-configuration-example.jpg)](https://thepracticaldeveloper.com/2018/11/24/spring-boot-kafka-config/)

## Multiple serialization / deserialization formats

To illustrate the different configuration options, this application deserializes Kafka messages in three different ways:

* As a JSON to Java object.
* As a simple String (plain JSON).
* As a byte array.
