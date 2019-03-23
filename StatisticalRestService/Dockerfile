FROM openjdk:13-ea-9-jdk-alpine3.9
EXPOSE 8080
CMD mkdir /opt/StatisticalRestService
COPY target/StatisticalRestService-0.0.1-SNAPSHOT.jar /opt/StatisticalRestService/
COPY DockerConfig/application.yml /opt/StatisticalRestService/
RUN chmod 777 /opt/StatisticalRestService/StatisticalRestService-0.0.1-SNAPSHOT.jar \
&& ls -l /opt/StatisticalRestService/StatisticalRestService-0.0.1-SNAPSHOT.jar 
ENTRYPOINT [ "java", "-jar", "-Dspring.config.location=/opt/StatisticalRestService/application.yml", "/opt/StatisticalRestService/StatisticalRestService-0.0.1-SNAPSHOT.jar" ]  