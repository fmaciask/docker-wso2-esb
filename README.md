ESB
===

Docker image to install and run WSO2 Enterprise Service Bus. 

### Usage
* To pull the latest version: `docker pull jgpelaez/wso2-esb`
* To build: `docker build --rm -t wso2esb 4.8.1/`
* To run: `docker run --rm --name wso2esb -p 9443:9443 wso2esb`

* To run the samples: `docker run -p 9443:9443 fmaciask/wso2-esb /opt/wso2esb-4.8.1/bin/wso2esb-samples.sh -sn <n>`

* To access ESB web admin console, navigate to `https://localhost:9443`
