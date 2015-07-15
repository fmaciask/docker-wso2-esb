FROM java:openjdk-8-jre

MAINTAINER juancarlosgpelaez@gmail.com

ENV WSO2_URL=https://s3-us-west-2.amazonaws.com/wso2-stratos
ENV WSO2_SOFT_VER=4.8.1
RUN  \
	mkdir -p /opt/wso2 && \
	wget -P /opt/wso2 $WSO2_URL/wso2esb-$WSO2_SOFT_VER.zip && \
    unzip /opt/wso2/wso2esb-$WSO2_SOFT_VER.zip -d /opt/wso2 && \
    rm /opt/wso2/wso2esb-$WSO2_SOFT_VER.zip

# ESB https port
EXPOSE 9443
# ESB http pass-through transport port
EXPOSE 8280
# ESB https pass-through transport port
EXPOSE 8243

CMD ["/opt/wso2/wso2esb-4.8.1/bin/wso2server.sh"]