pipeline {
 tools{
        jdk 'JAVA_HOME_UBUNTU'
		maven 'M2_HOME'
	}	
    agent { label "ubuntuslave" }

    stages {
	
        stage("checkout") {
            steps {
                git 'https://github.com/Chinku-code/New-maven-project.git'
            }
        }
		 stage("compile") {
            steps {
                sh 'mvn compile'
            }
        }
		 stage("test") {
            steps {
                sh 'mvn test'
            }
        }
		 stage("package") {
            steps {
                sh 'mvn package'
            }
        }
    }
}
