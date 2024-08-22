# sb-kafka-producer

Como utilizar:

### Inicializar o Zookeeper e o Kafka através do terminal no IntelliJ:

- Navegar até onde o Kafka está (Downloads)
- Executar o seguinte comando: bin/zookeeper-server-start.sh config/zookeeper.properties
- Em outro terminal, navegar até onde o Kafka está novamente (Downloads)
- Executar o seguinte comando: bin/kafka-server-start.sh config/server.properties
- Após isso, caso queira garantir que o tópico foi criado, navegar até onde o Kafka está e executar o seguinte comando:
bin/kafka-topics.sh --bootstrap-server=localhost:9092 --list

### Inicializar as duas aplicações (Consumer e Producer):

https://github.com/brujp/sb-kafka-consumer
https://github.com/brujp/sb-kafka-producer

### Criar uma request no Insomnia:

**POST** para localhost:9090/pagamentos

Body:

{
"numero": 3,

"valor": 300,

"descricao": "Debito de compra"
}
