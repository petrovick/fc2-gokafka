# Rodando a aplicação

```
docker-compose up -d
```

### Entrando na aplicação
```
docker exec -it gokafka bash
```

## Criando tópico
```
docker exec -it 3consumerproducer-kafka-1 bash
```

### Criando tópico
```
kafka-topics --bootstrap-server=localhost:9092 --create --topic=teste --partitions=3
```

### criando consumer
```
kafka-console-consumer --bootstrap-server=localhost:9092 --topic=teste
```