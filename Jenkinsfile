pipeline {
  agent any
  tools { 
        maven 'maven-3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp -Dsonar.organization=asgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9325586a8f1d1adf470b908a46156f5844'
			}
        } 
  }
}
