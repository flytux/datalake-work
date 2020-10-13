FROM confluentinc/cp-kafka-connect:5.5.0

RUN confluent-hub install --no-prompt confluentinc/kafka-connect-jdbc:5.5.0
RUN confluent-hub install --no-prompt confluentinc/kafka-connect-datagen:0.3.2
RUN echo "Downloading JDBC drivers"
COPY ./jdbc-drivers/* /usr/share/confluent-hub-components/confluentinc-kafka-connect-jdbc/lib/
#RUN apt-get update
#RUN apt-get install -y --force-yes unzip libaio1
#RUN wget "https://download.oracle.com/otn_software/linux/instantclient/19600/instantclient-basiclite-linux.x64-19.6.0.0.0dbru.zip" -O /tmp/ic.zip
#RUN unzip /tmp/ic.zip -d /usr/share/java/debezium-connector-oracle/
#RUN /etc/confluent/docker/run & sleep infinity
