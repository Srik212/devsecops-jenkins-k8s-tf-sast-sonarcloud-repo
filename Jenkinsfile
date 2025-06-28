pipeline {
  agent any
  tools { 
        maven 'Maven _3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopswebapp-2025_devsecops-project -Dsonar.organization=devsecopswebapp-2025 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=166929c981263f9e0aeeb556521d4c681a0d4c2c'
			}
        } 
  }
}
