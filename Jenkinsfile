node {
  def myGradleContainer = docker.image('gradle:jdk11')
  myGradleContainer.pull()
  stage('prep') {
    checkout scm
  }
  stage('test') {
     
       bat 'cd complete && gradle test'
    
  }
  stage('run') {
     
       bat 'cd complete && gradle run'
     
  }
}
