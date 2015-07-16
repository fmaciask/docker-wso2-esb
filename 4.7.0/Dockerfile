FROM java:openjdk-7

MAINTAINER juancarlosgpelaez@gmail.com

ENV WSO2_URL=http://dist.wso2.org/maven2/org/wso2/esb/wso2esb
ENV WSO2_SOFT_VER=4.7.0
RUN  \
	mkdir -p /opt && \
	wget -P /opt $WSO2_URL/$WSO2_SOFT_VER/wso2esb-$WSO2_SOFT_VER.zip && \
    unzip /opt/wso2esb-$WSO2_SOFT_VER.zip -d /opt && \
    rm /opt/wso2esb-$WSO2_SOFT_VER.zip

# ESB https port
EXPOSE 9443
# ESB http pass-through transport port
EXPOSE 8280
# ESB https pass-through transport port
EXPOSE 8243

ENV JAVA_HOME=/usr
CMD ["/opt/wso2esb-4.7.0/bin/wso2server.sh"]