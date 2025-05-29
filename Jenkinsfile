pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ndzamngangbuggywebapp_ndzamngangbuggywebapp -Dsonar.organization=ndzamngangbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6bf32517a83ff02a37770c5d8a953f5788db8047'
			}
        } 
  }
}
