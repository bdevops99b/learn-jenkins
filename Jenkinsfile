pipeline {
  agent {
    node {
      label 'workstation'
    }
  }

   options {
          ansiColor('xterm')
      }
  environment {
      sample_url="example.com"
  }
  stages
  {
    stage('One')
      {
         steps
            {
                sh 'echo Hello World'
                sh 'echo hello univ'
                sh 'echo ${sample_url}'
            }
      }
 }
post {
 always {
      sh 'echo Post Cleanup step'
      }
   }
}

