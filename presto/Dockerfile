FROM armhf/ubuntu:16.04
RUN apt-get update && apt-get install -y openjdk-8-jdk python less 
ADD http://maven.aliyun.com/nexus/service/local/repositories/central/content/com/facebook/presto/presto-server/0.187/presto-server-0.187.tar.gz /root/presto-server-0.187.tar.gz
RUN cd /root && tar -xzvf presto-server-0.187.tar.gz
ENTRYPOINT /root/presto-server-0.187/bin/launcher run
