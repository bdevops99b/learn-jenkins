// pipeline {
//   agent {
//     node {
//       label 'workstation'
//     }
//   }

//
 triggers {
//         pollSCM('H/2 * * * *')
//     }
//    options {
//           ansiColor('xterm')
//       }
//        parameters {
//            string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
//            }
//   environment {
//       sample_url="example.com"
//   }
//   stages
//   {
//     stage('One')
//       {
//           input {
//                message "Do you approve?"
//                ok "Yes"
//
//                 }
//          steps
//             {
//                 sh 'echo Hello World'
//                 sh 'echo hello univ'
//                 sh 'echo ${sample_url}'
//                 sh 'echo PERSON - ${PERSON}'
//             }
//       }
//       stage('Two')
//             {
//              when {
//              expression {
//                    GIT_BRANCH == "origin/test"
//                  }
//             }
//             steps {
//             sh 'env'
//            }
//             }
//  }
// post {
//  always {
//       sh 'echo Post Cleanup step'
//       }
//    }
// }

pipeline {
agent any
stages {
stage('Parallel') {
parallel
{
stage('One') {
  steps {
      sh 'echo one'
     }
  }
  stage('Two') {
  steps {
      sh 'echo two'
     }
  }
    stage('Three') {
    steps {
        sh 'echo three'
       }
    }
}

}

}

}