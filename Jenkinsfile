pipeline {
    agent {
   label '24thlinuxnode'
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
  sh "cd /home/ubuntu/workspace/24thlinuxnode/testing@script ; mvn clean install"
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
              echo 'Deploy.Hello world'
 }
}
    }
}
