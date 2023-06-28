# Replace "kafka-console-consumer.sh" by "kafka-console-consumer" or "kafka-console-consumer.bat" based on your system # (or bin/kafka-console-consumer.sh or bin\windows\kafka-console-consumer.bat if you didn't setup PATH / Environment variables)

```console
kafka-console-consumer.sh 
```

# consuming
```console
kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic first_topic
```

# other terminal
```console
kafka-console-producer.sh --bootstrap-server localhost:9092 --topic first_topic
```

# consuming from beginning
```console
kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic first_topic --from-beginning
```

# display key, values and timestamp in consumer
```console
kafka-console-consumer --bootstrap-server localhost:9092 --topic first_topic --formatter kafka.tools.DefaultMessageFormatter --property print.timestamp=true --property print.key=true --property print.value=true --from-beginning
```