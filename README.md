# Ilan Matific Technical Tasl
## Overview
1. To start with This project consists of a bootstrap script that does the following,

* Install all required toolset [kind, kubectl, helm]
* Creates a kubernetes cluster
* Deploys Jenkins server
* Deploys Postgres database
* Deploys Django app

### Kubernetes / Django / Jenkins
* This single command will take awhile to run as it does quite a few items,

```
./bootstrap.sh
```

2. Next step is to Install Docker

$ sudo apt-get update
$ sudo apt-get install ca-certificates curl gnupg lsb-release #### setup docker apt repository
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpgecho \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null#### install docker packages
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io #### test your installation
sudo docker run hello-world


## Prerequisites
* [Git](https://git-scm.com/) >= 2.19.1
* [Ubuntu](https://www.ubuntu.com/) >= 20 LTS
* Clone this repository to you local.
* [JenkinsSetup] Installed Jenkins needed to be configured to set up the webhook to the preferred repository.
* [JenkinsFile] Jenkinsfile need to be modified with your repository URL and in the same file Docker Ip address need to changed using your local ip address
* Internet access - as it relies heavy on publicly available bitnami helm charts

## Development
### Improvments
Quite a few improvements are identified. It will be actioned. Contributions welcome.

## Authors
* Ilan Durairaj
