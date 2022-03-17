pipeline{
  
    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven 'maven'
    }


    stages{
        stage('build'){
            steps{
                echo '1 this is the build job'
                sh 'mvn compile'
            }
        }
        stage('test'){
            steps{
                echo '2 this is the test job'
                sh 'mvn clean test'
            }
        }
        stage('package'){
            steps{
                echo '3 this is the package job'
                sh 'mvn package -DskipTests'
            }
        }
    }

  }
