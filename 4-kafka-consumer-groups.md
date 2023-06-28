 # Replace "kafka-consumer-groups.sh" by "kafka-consumer-groups" or "kafka-consumer-groups.bat" based on your system # (or bin/kafka-consumer-groups.sh or bin\windows\kafka-consumer-groups.bat if you didn't setup PATH / Environment variables)

# documentation for the command 
```console
kafka-consumer-groups.sh 
```

# list consumer groups
```console
kafka-consumer-groups.sh --bootstrap-server localhost:9092 --list
```

# describe one specific group
```console
kafka-consumer-groups.sh --bootstrap-server localhost:9092 --describe --group my-second-application
```

# describe another group
```console
kafka-consumer-groups.sh --bootstrap-server localhost:9092 --describe --group my-first-application
```

# start a consumer
```console
kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic first_topic --group my-first-application
```

# describe the group now
```console
kafka-consumer-groups.sh --bootstrap-server localhost:9092 --describe --group my-first-application
```

# describe a console consumer group (change the end number)
```console
kafka-consumer-groups.sh --bootstrap-server localhost:9092 --describe --group console-consumer-10592
```

# start a console consumer
```console
kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic first_topic --group my-first-application
```

# describe the group again
```console
kafka-consumer-groups.sh --bootstrap-server localhost:9092 --describe --group my-first-application
```