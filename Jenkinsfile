pipeline{
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
          stage('Build'){
            steps {
                echo 'Hello World'
            }
        }
        stage('Test'){
            steps {
                echo 'Hello World'
            }
        }
        stage('Run') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Hello World'
            }
        }
    }
    post{ always {echo 'I will always say hello again'}}
}

}
