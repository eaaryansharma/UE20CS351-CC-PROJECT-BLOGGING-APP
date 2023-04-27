## Team Members:
```
AARYAN SHARMA   PES1UG20CS003
ABHISHEK        PES1UG20CS010
ADITYA N        PES1UG20CS021
ALOK KUMAR      PES1UG20CS032
```


## Problem Statement
Microservices are an architectural and organizational approach to software development where software is composed of small independent services that communicate over well-defined APIs. Microservices architectures make applications easier to scale and faster to develop, enabling innovation and accelerating time-to-market for new features.
Docker and Kubernetes are almost synonymous to 'microservices' as they help package and manage the different components of a project/ application, thereby easing up the implementation of a microservices architecture.

**In this project,we have worked with Docker and Kubernetes to make an easily deployable and portable blogging web-app using Flask and MongoDB.**  

The microservices architecture will deploy a Kubernetes cluster with a mongodb server pod fronted with a web admin interface and a pod to run the flask app.

## Pre-Requisites/ Pre-Installation:
1. Docker ([Windows](https://docs.docker.com/desktop/windows/install/) | [Ubuntu](https://docs.docker.com/engine/install/ubuntu/#:~:text=Install%20from%20a%20package&text=Go%20to%20https%3A%2F%2Fdownload,version%20you%20want%20to%20install) | [MacOS](https://docs.docker.com/desktop/mac/install/))
2. Kubernetes ([Windows](https://birthday.play-with-docker.com/kubernetes-docker-desktop/) | [Ubuntu](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/) | [MacOS](https://birthday.play-with-docker.com/kubernetes-docker-desktop/))

## File Structure
```
.
|-- README.md
|-- app
|   |-- app.py
|   |-- requirements.txt
|   `-- templates
|       |-- base.html
|       |-- create-post.html
|       |-- edit-post.html
|       |-- home.html
|       `-- searchauthor.html
|-- configmap.yaml
|-- deployments.yaml
|-- flask-app-image.dockerfile
|-- secret.yaml
`-- services.yaml
```
The `app` directory contains all the code pertaining to the flask app. 
The `.yaml` files in the root directory are to specify the kubernetes manifests that will bring up your microservices deployment of the problem statement. 

## Output Screenshot
1. The Home Page displaying all the posts.
<p align = "center">
    <img src = "https://user-images.githubusercontent.com/114352512/233695944-d5477d17-88a0-4735-afcf-91f130223a4d.jpg"/>
</p>

2. You can view the database frontend exposed by mongo-express. To do so, on your browser, navigate to`EXTERNAL_IP:port` exposed by the mongo-express service. Here is the sample output:  

<p align = "center">
    <img src = "https://user-images.githubusercontent.com/56164920/158070411-3dff479d-ee7f-4eeb-b38f-92ccc221c6aa.png"/>
</p>

## All Done! :)
# UE20CS351-CC-PROJECT-BLOGGING-APP
