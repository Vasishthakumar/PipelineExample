pipeline { 
    agent any  
    stages { 
        stage('Build') { 
            steps { 
               echo 'Maven Test, Compile and Packaging using jenkinsfile .' 
              
            }
        }
        stage('Compile') { 
            steps { 
               bat 'mvn clean compile'
            }
		}
		stage('Test') {
            steps {
                bat 'mvn clean test'
            }
        }		
		stage('Install') {
            steps {
                bat 'mvn clean install'
            }
        }
    }
}
