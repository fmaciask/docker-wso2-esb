FROM java:openjdk-8-jre

# Maintainer
MAINTAINER Juan Carlos García Peláez

RUN  \
	mkdir -p /opt/wso2 && \
	wget -P /opt/wso2 http://dist.wso2.org/maven2/org/wso2/esb/wso2esb/4.8.0/wso2esb-4.8.0.zip && \
    unzip /opt/wso2/wso2esb-4.8.0.zip -d /opt/wso2 && \
    rm /opt/wso2/wso2esb-4.8.0.zip

EXPOSE 9443
CMD ["/opt/wso2esb-4.8.0/bin/wso2server.sh"]


