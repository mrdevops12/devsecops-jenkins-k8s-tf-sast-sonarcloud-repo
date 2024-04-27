pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=testing-devsec -Dsonar.organization=testing-devsec -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=0c4aff24e69fdd93c950fa541bbfaee291f45b31'
			}
        } 
  }
}
