FROM centos:7

RUN (cd /opt && \
curl -L -b "oraclelicense=a" http://download.oracle.com/otn-pub/java/jdk/8u131-b11/d54c1d3a095b4ff2b6607d096fa80163/jdk-8u131-linux-x64.tar.gz -O && \
tar xzf jdk-8u131-linux-x64.tar.gz && \
cd /opt/jdk1.8.0_131/ && \
alternatives --install /usr/bin/java java /opt/jdk1.8.0_131/bin/java 2 && \
alternatives --install /usr/bin/jar jar /opt/jdk1.8.0_131/bin/jar 2 && \
alternatives --install /usr/bin/javac javac /opt/jdk1.8.0_131/bin/javac 2 && \
alternatives --set jar /opt/jdk1.8.0_131/bin/jar && \
alternatives --set javac /opt/jdk1.8.0_131/bin/javac && \
echo "export JAVA_HOME=/opt/jdk1.8.0_131" >> /etc/bashrc && \
echo "export JRE_HOME=/opt/jdk1.8.0_131/jre" >> /etc/bashrc && \
echo "export PATH=$PATH:/opt/jdk1.8.0_131/bin:/opt/jdk1.8.0_131/jre/bin" >> /etc/bashrc && \
rm -v /opt/jdk-8u131-linux-x64.tar.gz )
