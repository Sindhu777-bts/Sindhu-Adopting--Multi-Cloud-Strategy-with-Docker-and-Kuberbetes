# CI-CD-Pipeline
Real time webapp deployment on Kubernetes cluster using Jenkins CI/CD pipeline.

# INTRODUCTION TO DOCKER
Docker is an open platform for developing, shipping, and running applications. Docker enables you to separate your applications from your infrastructure so you can deliver software quickly. Docker is a software platform that allows you to build, test, and deploy applications quickly. Docker packages software into standardized units called containers that have everything the software needs to run including libraries, system tools, code, and runtime.Docker registries are used to host and distribute Docker Images. Docker Hub is Docker's official cloud-based registry. The free version of Docker Hub allows for one private repository. Nonpaying users are otherwise restricted to public repositories. .


![image alt](https://github.com/Sindhu777-bts/Sindhu-Adopting--Multi-Cloud-Strategy-with-Docker-and-Kuberbetes/blob/0c97017a1cd494f4d80f69e4007a99f2d5fd0b19/WhatsApp%20Image%202025-02-21%20at%209.13.04%20PM.jpeg)

# PROJECT DESCRIPTION
* JENKINS
* ANSIBLE
* WEBAPP(Kubernetes cluster)

# WORKING
Firstly, developer writes the Docker File and push it to GITHUB Repository. If the git repository gets new commit, it will notify Jenkins through WEBHOOK to build that new code. JENKINS will PULL all the code from repository and SSH (secure shell) to the ANSIBLE SERVER in order to provide network communication and share data. ANSIBLE SERVER will firstly get the DockerFile and start build Image. Then, tag image and push it to DOCKER HUB. Ansible server will then SSH to KUBERNETES SERVER. Thereafter, Fetch the LATEST IMAGE which is just build and pushed. PULL from DOCKER HUB and build container from Image. This container must be accessible to us using IP and Port by writing service.mk in Kubernetes Cluster. A Kubernetes cluster is a set of nodes that run containerized applications. Containerizing applications packages an app with its dependences and some necessary services. They are more lightweight and flexible than virtual machines. Also, we maintain a image version as well as Separate latest Image with Build Number.
# DevOps Tools-
## JENKINS
A DevOps software development method called continuous integration involves developers regularly merging their code changes into a common repository, which is followed by the execution of automated builds and tests. Developers frequently utilise Jenkins, an Open-Source Continuous Integration (CI) tool, to automate the testing and deployment of their apps. A Webhook is a tool that enables a Jenkins project to be built automatically in response to a commit that is pushed to a Git repository.
## Ansible 
Ansible is defined as an open-source, cross-platform tool for resource provisioning automation that DevOps professionals popularly use for continuous delivery of software code by taking advantage of an “infrastructure as code” approach.
