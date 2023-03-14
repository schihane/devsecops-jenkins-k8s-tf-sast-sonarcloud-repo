pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp213 -Dsonar.organization=asgbuggywebapp213 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=6d7e4e552e896bfd3aa5918feccb536c77afa73c'
			}
        } 
  }
}
