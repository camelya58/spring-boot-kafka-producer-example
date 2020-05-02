# spring-boot-kafka-producer-example

it is necessary to set up consumer. 
download apache kafka
Terminal 1
bin/zookeeper-server-start.sh config/zookeeper.properties

Terminal 2
bin/kafka-server-start.sh config/server.properties

Terminal 3
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example

bin/kafka-console-consumer.sh -- bootstrap-server localhost:9092 --topic Kafka_Example --from-beginning 
