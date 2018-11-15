FROM chp/java

RUN (mkdir -p /opt && \
cd /opt && \
curl http://apache.cs.uu.nl/hadoop/common/hadoop-3.1.1/hadoop-3.1.1.tar.gz -O && \
tar zxf hadoop-3.1.1.tar.gz && \
rm -v /opt/hadoop-3.1.1.tar.gz && \
echo "export PATH=$PATH:/opt/hadoop-3.1.1/bin" >> /etc/bashrc && \
echo "export HADOOP_CONF_DIR=$PATH:/etc/hadoop" >> /etc/bashrc )
