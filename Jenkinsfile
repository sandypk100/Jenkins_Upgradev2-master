pipeline {
      agent any
      stages {
            stage('Build Application') {
                  steps {
                        echo 'Hi, this is Anshul from LevelUp360'
                        echo 'Building Sample Maven Project'
                        sh 'mvn clean package'
                        
                  }
                  post{
                        success{
                              echo 'Now archiving the artifacts'
                              archiveArtifacts artifacts: '**/*.war'
                              
                              
                        }
                        
                  }      
            }
            
            
      }
}
