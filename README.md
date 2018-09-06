# kafka_producer_demo
This Project covers how to use Spring Boot with Spring Kafka to Consume JSON/String message from Kafka topics

<h2>Start Zookeeper</h2>

zkserver

<h2>Start Kafka Server</h2>

.\bin\windows\kafka-server-start.bat .\config\server.properties

<h2>Create Kafka Topic</h2>

.\kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic test


<h2>Publish to the Kafka Topic via Console</h2>

.\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic Kafka_Demo --from-beginning
