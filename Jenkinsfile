pipeline 
{
agent any
  stages 
    {
    stage ('Source Composition Analysis') 
      {
      steps 
      	 { 
        dependencyCheck additionalArguments: '', odcInstallation: 'ODC_Check'
        dependencyCheckPublisher pattern: 'dependency-check-report.xml' 
        sh 'mv dependency-check-report.xml /var/jenkins_home/workspace/ODC_SCA/reports' 
        }
      }
    }
  }