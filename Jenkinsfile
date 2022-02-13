pipeline {
  agent "jenkins-slave-1"
  stages{
    stage("build"){
      steps{
        //sh "sudo docker container stop aswin/website:v1"
        sh "sudo docker build -t aswin/website:v1 ."
        sh "sudo docker run -p 80:80 -d aswin/website:v1"
      }
    }
  }
}
