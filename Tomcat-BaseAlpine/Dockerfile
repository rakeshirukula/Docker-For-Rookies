FROM alpine:3.14
RUN apk update && \ --no-install-recommends 
    apk add openjdk11 && \
    rm -rf /var/lib/apt/lists/*
ENV JAVA_HOME /usr/lib/jvm/default-jvm    
EXPOSE 8080
COPY . /opt/
ENTRYPOINT ["/opt/apache-tomcat-10.1.17/bin/catalina.sh","run"]