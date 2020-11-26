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
        
        stage('Build') {
            steps {
                echo 'Hello World'
            }
        }
         node('Ubuntu24node'){
         stage('test') {
            steps {
                echo 'this is the test stage which runs on different node'
            }
        }
         }
         stage('Run') {
            steps {
                echo 'This is the run the build stage'
            }
         }
         stage('Deploy') {
            steps {
                echo 'this is the deployment stage'
            }
        }

    }
}
