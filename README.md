# Nodejs-test

For accessing the image: 

#aws configure with provided access key id and secret ket  and then run secret.sh key for generating ImagePullSecret/

***nodejs-test:latest image hosted at AWS ECR, below is the URI:

986304663873.dkr.ecr.us-east-2.amazonaws.com/nodejs-test:latest

Load Balancer IP:

http://nginx-lb-266136591.us-east-2.elb.amazonaws.com:3000/

===================================


deployment.yml ----> Creates a deployment names "application" with 10 replicas,makes sure at least 7 pods are running at any given time during the change in deployment.

service.yml    ----> Creates a sercvice which exposes the container pod to  NodePort.

horizontalPodsAutoscaler.yml	---> Creates a hpa which scales up the deployment whenever CPU and Memory utilizations go beyond the defined limits.





