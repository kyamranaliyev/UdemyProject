pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp12345 -Dsonar.organization=asgbuggywebapp12345 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=c8f4ce9337b5c51a5e4d27a5882d2749e2a59074'
			}
        }
  }
}
