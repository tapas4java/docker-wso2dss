docker-wso2dss
==============

Docker Image for WSO2 Data Services Server(DSS).

The dockerfile will:

* Copy `DSS 4.9.0 zip` to /otp from Packages directory.
* Unzip the DSS 4.9.0 ZIP.
* Expose the container port `9443`.
* Set the DSS `wso2server.sh` start-up script as the container start-up command.

### Usage
* To pull: `docker pull anitech/wso2-dss`
* To build: `docker build -t your_image_name github.com/tapas4java/docker-wso2dss`
* To run: `docker run --rm --name your_container_name -p 9443:9446 your_image_name`
* To access DSS web admin console, navigate to `https://localhost:9446`