# Feel The Four Website and Webstore Production
<https://www.feelthefourrecords.com/> \
By Jarrett Dougherty

## Description
This repository is used to deploy the frontend and backend code located at <https://github.com/JarrettD5309/ftfstore> \

## Instructions
* A `.env` file must be created with a Stripe Key.
* The `/out` folder and the JAR file must be manually copied into this repository from the `ftfstore` repository. There are currently no CI/CD configurations.
* To run the server, use the command `java -cp ftfstore-1.0-SNAPSHOT-jar-with-dependencies.jar com.feelthefour.ftfstore.App` from the root directory. This will serve the site at `localhost:7070`.