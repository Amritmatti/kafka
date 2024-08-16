```docker exec --workdir /opt/kafka/bin/ -it broker-1 ./kafka-topics.sh --bootstrap-server broker-1:19092,broker-2:19092,broker-3:19092 --create --topic test-topic
docker exec --workdir /opt/kafka/bin/ -it broker-1 ./kafka-console-producer.sh --bootstrap-server broker-1:19092,broker-2:19092,broker-3:19092 --topic test-topic
docker exec --workdir /opt/kafka/bin/ -it broker-1 ./kafka-console-consumer.sh --bootstrap-server broker-1:19092,broker-2:19092,broker-3:19092 --topic test-topic --from-beginning



docker exec --workdir /opt/kafka/bin/ -it broker-1 ./kafka-topics.sh --create --bootstrap-server broker-1:9092,broker-2:19092,broker-3:19092 --replication-factor 3 --partitions 9 --topic test1_skh3
docker exec --workdir /opt/kafka/bin/ -it broker-1 ./kafka-topics.sh --bootstrap-server broker-1:9092,broker-2:19092,broker-3:19092 --list
docker exec --workdir /opt/kafka/bin/ -it broker-1 ./kafka-console-producer.sh --bootstrap-server broker-1:19092,broker-2:19092,broker-3:19092 --topic test1_skh3
docker exec --workdir /opt/kafka/bin/ -it broker-1 ./kafka-console-consumer.sh --bootstrap-server broker-1:19092,broker-2:19092,broker-3:19092 --topic test1_skh3 --from-beginning
```
