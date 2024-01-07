FROM amazonlinux
MAINTAINER RAKESH
EXPOSE 8080
RUN yum update -y && \
    yum install -y java-11-amazon-corretto-headless  --allowerasing && \
    yum clean all
ENV JAVA_HOME /usr/lib/jvm/java-11-amazon-corretto
COPY . /opt/
ENTRYPOINT ["/opt/apache-tomcat-10.1.17/bin/catalina.sh","run"]