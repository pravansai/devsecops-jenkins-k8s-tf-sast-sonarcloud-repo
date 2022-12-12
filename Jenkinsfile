pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=saibugapp -Dsonar.organization=saibugapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=231fd4d055ec1bb30848d51fce643a9b982999ca'
			}
        } 
  }
}
