pipeline 
{
agent any
  stages 
    {
    stage ('Source Composition Analysis') 
      {
      steps 
      	 { 
        dependencyCheck additionalArguments: '', odcInstallation: 'ODC'
        dependencyCheckPublisher pattern: 'dependency-check-report.html' 
        sh 'mv dependency-check-report.html /var/jenkins_home/workspace/ODC_SCA/reports' 
        }
      }
    }
  }
