pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sec-guru_buggywebappnew -Dsonar.organization=sec-guru -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=832bfb68ec41bed847e2d9dadcb79cca4a159120'
			}
        } 
  }
}
