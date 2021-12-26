# mule-aws-ecs-app
Simple mule application to demonstrate the docker image deployment on AWS ECS Fargate instance. 

Build mule application in command line using below command

`mvn clean package`

To build docker image, run below command -

`docker build . -t mule-aws-ecs-app:latest`

To run above docker image, run below command -

`docker run -it --rm -p 8080:8080 mule-aws-ecs-app:latest`

Once the application is running use below URLs to access Mule console & API-

http://localhost:8081/console
http://localhost:8080/api/hello?firstName=Vishnu
