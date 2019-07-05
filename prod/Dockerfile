FROM alpine:latest
RUN apk update && apk add openjdk8 wget tar \
&& mkdir -p /usr/local/tomcat8 \
&& cd /usr/local/tomcat8 \
&& wget http://apache-mirror.rbc.ru/pub/apache/tomcat/tomcat-8/v8.5.42/bin/apache-tomcat-8.5.42.tar.gz \
&& tar xvzf apache-tomcat-8.5.42.tar.gz --strip-components 1
CMD ["/usr/local/tomcat8/bin/catalina.sh", "run"]
