FROM java:17
ADD config-server.0.0.1.jar app.jar
VOLUME /tmp
VOLUME /target
RUN bash -c 'touch /app.jar'

EXPOSE 8888
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]