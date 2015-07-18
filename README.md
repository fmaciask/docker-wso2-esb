ESB
===

Docker image to install and run WSO2 Enterprise Service Bus. 

### Usage
* To pull the latest version: `docker pull jgpelaez/wso2-esb`
* To pull a concrete version: `docker pull jgpelaez/wso2-esb:version`
* To build: `docker build --rm -t your_image_name github.com/jgpelaez/docker-wso2esb`
* To run: `docker run --rm --name your_container_name -p 9443:9443 your_image_name`

* To run the samples: `docker run -p 9443:9443 jgpelaez/wso2-esb /opt/wso2esb-4.8.1/bin/wso2esb-samples.sh -sn <n>`

* To access ESB web admin console, navigate to `https://localhost:9443`
