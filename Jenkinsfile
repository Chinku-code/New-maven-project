pipeline {
 tools{
        jdk 'JAVA_HOME_WIN'
		maven 'M2_HOME_WIN'
	}	
    agent { lable "winslave" }

    stages {
	
        stage("checkout") {
            steps {
                git 'https://github.com/Chinku-code/New-maven-project.git'
            }
        }
		 stage("compile") {
            steps {
                bat 'mvn compile'
            }
        }
		 stage("test") {
            steps {
                bat 'mvn test'
            }
        }
		 stage("package") {
            steps {
                bat 'mvn package'
            }
        }
    }
}
