FROM ubuntu:16.04
RUN apt-get update && apt-get install git maven default-jdk -y \
&& echo "#!/bin/bash" > script.sh \
&& echo "git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git && cd boxfuse-sample-java-war-hello/ && mvn package && cd target/ && mkdir -p /package && cp hello-1.0.war /package" >> script.sh \
&& chmod +x script.sh
CMD ["./script.sh"]
