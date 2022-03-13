node{

  git branch: "master", url: "https://github.com/CHEZHIA75/IlanMatific" 

  stage ('Build the Docker image') {
    sh "echo building the image..."
    sh "docker build --tag django_test:latest ."
    sh "echo building image complete."

  }

  stage ('Deploy the Docker image') {
    sh "echo Deploying the container..."
    sh " docker rm -f django_test"
    sh "docker run -d -p 192.168.163.74:8000:8000 --name django_test  django_test:latest "
    sh "echo Container successfully deployed."

  }

}