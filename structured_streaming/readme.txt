# Start zookeeper
bin/zookeeper-server-start.sh config/zookeeper.properties

# Start kafka server
JMX_PORT=8004 bin/kafka-server-start.sh config/server.properties

# Create topic
bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic spark-streaming

Dataset link:
https://www.kaggle.com/datasets/ealaxi/paysim1/
Downlaod the dataset and then add a folder as data and then add the files
