pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebappparsi -Dsonar.organization=buggywebappparsi -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=32bf2062ae3079f3226a5601cb3b063aac086cb3'
			}
        } 
  }
}
