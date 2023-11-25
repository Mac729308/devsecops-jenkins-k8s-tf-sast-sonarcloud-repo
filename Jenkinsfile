pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp121 -Dsonar.organization=asgbuggywebapp121 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b2cb47705649e2f3b976d26cb1d0830b5f3d7a69'
			}
        } 
  }
}
