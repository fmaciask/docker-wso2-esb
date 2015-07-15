FROM java:openjdk-7

MAINTAINER juancarlosgpelaez@gmail.com

ENV WSO2_URL=http://dist.wso2.org/maven2/org/wso2/esb/wso2esb
ENV WSO2_SOFT_VER=4.5.0
RUN  \
	mkdir -p /opt/wso2 && \
	wget -P /opt/wso2 $WSO2_URL/$WSO2_SOFT_VER/wso2esb-$WSO2_SOFT_VER.zip && \
    unzip /opt/wso2/wso2esb-$WSO2_SOFT_VER.zip -d /opt/wso2 && \
    rm /opt/wso2/wso2esb-$WSO2_SOFT_VER.zip

# ESB https port
EXPOSE 9443
# ESB http pass-through transport port
EXPOSE 8280
# ESB https pass-through transport port
EXPOSE 8243

ENV JAVA_HOME=/usr
CMD ["/opt/wso2/wso2esb-4.5.0/bin/wso2server.sh"]