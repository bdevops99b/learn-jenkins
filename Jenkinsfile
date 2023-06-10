pipeline {
  agent any
  stages
  {
  stage('One')
  {
  steps
  {
  sh 'echo Hello World'
  sh " echo hello univ"
  }
}
}
post {
 always {
      sh 'echo Post Cleanup step'
      }
   }
}

