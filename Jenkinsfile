pipeline {
  agent any
  stages{
    stage("build"){
      steps{
        script{
          //sh "sudo docker container stop aswin/website:v1"
          sh("sudo docker build -t aswin/website:v1 . && sudo docker run -p 80:80 -d aswin/website:v1")
        }
      }
    }
  }
}
