# stock-predictor 
## stock prediction app using prophet and yahoo finance

curl \
--header "Content-Type: application/json" \
--request POST \
--data '{"ticker":"MSFT", "days":7}' \
http://35.163.200.64:8000/predict

## What does it mean to create a Docker image and why do we use Docker images?
### Creating a docker image means packaging all the necessary components to run an app into a single unit. We use docker images to port apps between platforms. Also using a docker image we can scale an app to run on multiple platforms/environments and we can make sure the app stays consistent across the apps. Last, Docker images provide a much safer medium to deploy apps as security issues can be caught early on. 


## Please explain what is the difference from a Container vs a Virtual Machine? 
### A Virtual Machine (VM) is a complete software emulation of a  physical computer on a host motion. Thus allowing to run multiple virtual computers on a physical computer. A container uses the kernel and OS of the hosting machine to emulate only the components that are necessary to run the app. Thus it is less safe than VM but much more efficient.  

## What are 5 examples of container orchestration tools (please list tools)? 
### Nomad, Docker Swarm, Amazon ECS, Kubernetes, Apache Mesos

## How does a Docker image differ from a Docker container?
### Adocker container holds everything needed to run an app including the app itself. A Docker image is a snapshot of the container at a given instance in time. Thus it cannot run the app by itself but can give the requirements needed to run the app and a certain idea of what it looks like in real time.

 



