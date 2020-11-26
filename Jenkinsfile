pipeline {
    agent {
   label 'Ubuntu24node'
    }
       
    stages
    {
        stage('checkout')
        {
            steps {
                checkout scm
        }
    }
     stage('Build')
{
  steps
{
  sh "cd /home/ubuntu/workspace/Ubuntu24node/testing ; mvn clean install"
}
}
  stage('Test')
     {
          steps
{
             echo 'test.Hello world'
 }
}
        stage('Build')
     {
          steps
{
             echo 'build.Hello world'
 }
}
        stage('Run')
     {
          steps
{
             echo 'Run.Hello world'
 }
}
        stage('Deploy')
     {
          steps
{
    node ('24thlinuxnode') {
          
             echo 'Deploy.Hello world'
 }
}
    }
}
}
