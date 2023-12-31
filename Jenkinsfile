pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=adrielletest_adrielletest -Dsonar.organization=adrielletest -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=024a6e714a42cdc8962390d58caa4d073fe5a589'
			}
        } 
  }
}
