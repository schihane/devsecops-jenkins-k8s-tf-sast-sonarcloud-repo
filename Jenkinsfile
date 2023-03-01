pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp69 -Dsonar.organization=vinnie -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=dfe059463e33aab011417044591006fd1f672e5a'
			}
        } 
  }
}
