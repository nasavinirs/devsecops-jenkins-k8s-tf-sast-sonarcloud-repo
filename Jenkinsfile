pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileAndRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbugwebapp -Dsonar.organization=asgbugwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=543097f28d6669ee1487c0604c011a013af92020'
			}
        } 
  }
}
