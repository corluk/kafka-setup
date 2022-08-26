FROM eclipse-temurin:17.0.4.1_1-jre
WORKDIR /kafka-src
COPY kafka_2.12-3.2.1.tgz /tmp   
#COPY mount/config /opt/config 
RUN tar -xvf /tmp/kafka_2.12-3.2.1.tgz  
RUN ln -s /kafka-src/kafka_2.12-3.2.1 /kafka 
#RUN  rm /tmp/kafka_2.12.-3.2.1.tgz

RUN mkdir /tmp/zookeeper
#RUN mkdir /opt/config

CMD /kafka/bin/zookeeper-server-start.sh /config/zookeeper.properties
#RUN ln -s /kafka /zookeeper/kafka_2.12-3.2.1
#VOLUME [ "/kafka/kafka_2.12-3.2.1" ]
 #RUN  "tar -xvf /opt/kafka_2.12-3.2.1.tgz"
#RUN  "ln -s /opt/kafka_2.12-3.2.1 /opt/kafka" 

