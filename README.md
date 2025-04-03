# Feel The Four Website and Webstore Production
<https://www.feelthefourrecords.com/> \
By Jarrett Dougherty

## Description
This repository is used to deploy the frontend and backend code located at <https://github.com/JarrettD5309/ftfstore> \

## Instructions
* A `.env` file must be created in the root directory with a Stripe Key.
* The `/out` folder and the JAR file must be manually copied into this repository from the `ftfstore` repository. There are currently no CI/CD configurations.
* To run the server, use the command `java -cp ftfstore-1.0-SNAPSHOT-jar-with-dependencies.jar com.feelthefour.ftfstore.App` from the root directory. This will serve the site at `localhost:7070`.

## Deployment
* The site is deployed to a DigitalOcean Ubuntu server using Nginx.
* The Java process is being run using the command `nohup java -cp ftfstore-1.0-SNAPSHOT-jar-with-dependencies.jar com.feelthefour.ftfstore.App &` from the root of the project.
* The command `pgrep -a java` can be used to check the running process.
* The process can be stopped using the process ID reported from the previous `pgrep -a java` command. For example if the process ID is `1234` the command to stop the process would be `kill 1234`.