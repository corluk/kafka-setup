FROM eclipse-temurin:17.0.4.1_1-jre
WORKDIR /opt
RUN wget https://downloads.apache.org/kafka/3.2.1/kafka_2.12-3.2.1.tgz -O kafka.tgz 
RUN tar -xvf kafka.tgz  
RUN rm kafka.tgz 
RUN ln -s /opt/kafka_2.12-3.2.1 /kafka 
WORKDIR /kafka/bin
CMD /kafka/bin/kafka-server-start.sh /config/server.properties 