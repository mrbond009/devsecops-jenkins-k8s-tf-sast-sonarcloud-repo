pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ambeorgkey -Dsonar.organization=ambeorg -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9538160d96e029dda1ec63ae9c60ff3cbd70e529'
			}
        } 
  }
}
