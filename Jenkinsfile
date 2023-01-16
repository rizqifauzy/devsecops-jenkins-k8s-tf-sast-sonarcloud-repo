pipeline {
  agent any
  tools { 
        maven 'maven-3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=arf-attck-webapp -Dsonar.organization=arf-attck -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=67c391f24f7f77947fe60f984072bdb60dbf731b'
			}
        } 
  }
}
