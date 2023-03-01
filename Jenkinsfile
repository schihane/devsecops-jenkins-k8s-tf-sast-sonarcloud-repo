pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp69 -Dsonar.organization=vinnie -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=6cf2870019b80907697db61acca4445c7c9748a7'
			}
        } 
  }
}
