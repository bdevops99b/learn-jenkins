pipeline {
  agent {
    node {
      label 'workstation'
    }
  }

   options {
          ansiColor('xterm')
      }
       parameters {
           string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
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
                sh 'echo PERSON - ${PERSON}'
            }
      }
 }
post {
 always {
      sh 'echo Post Cleanup step'
      }
   }
}

