// Define variables
def _GATSBY_URL = "https://github.com/devopspwc/wptest"
def _PROJECT_URL = "github.com/pwc-doit/devops"
def _PROJECT_DIR = "grid"
def _DIR = "test-build-only"
def SURGE_LOGIN = "tommassie@hotmail.com"
def SURGE_DOMAIN = "tm008558.surge.sh"

// Work
pipeline {
   agent { label 'jenkins-aws' }
   triggers {
    GenericTrigger(
      genericVariables: [
        [key: 'ref', value: '$.ref']
      ],

      causeString: 'Triggered on $ref',

      token: 'LiHdVSYNri',
      //token: '',

      printContributedVariables: true,
      printPostContent: true,

      regexpFilterText: '', 
      regexpFilterExpression: ''
     )
     }
   stages {
//     stage('Create Project') {
//      steps {
//          sh label: '', script: """
//          node -v
//          gatsby -v
//          if [ -d "$_DIR" ]; then
//            echo "Removing existing project files."
//            rm -rf "$_DIR"
//            echo "Re-Loading Project"
//            gatsby new "$_DIR" "$_GATSBY_URL"
//          else
//            echo "Loading project"
//            gatsby new "$_DIR" "$_GATSBY_URL"
//          fi"""
//         }
//       }
//      stage('Build') {
//        steps {
//          dir ("${_DIR}") {
//           sh label: '', script: '''
//               gatsby build'''
//          }
//       }
//     }
//     stage('Release') {
//      steps {
//          withCredentials([string(credentialsId: 'surge_token', variable: 'surge_t')]) {
//          dir ("${env.WORKSPACE}/${_DIR}/public") {
//            sh label: '', script: """
//            echo 'machine surge.surge.sh
//                login tommassie@hotmail.com' | tee ~/.netrc
//            echo '    password' "$surge_t" | tee -a ~/.netrc
//            surge --project . --domain tm008558.surge.sh
//            """
//            }
//          }
//        }
//      }
//     stage('Clone Project') {
//      steps {
//        git credentialsId: 'fd41c67e-7760-4743-a88d-523b55ed54fa', url: 'https://github.com/pwc-doit/devops'
//        sh 'ls -l'
//        }
//      }
//    stage('Smoke') {
//      steps {
//        dir ("${env.WORKSPACE}/${_PROJECT_DIR}") {
//            sh label: '', script: '''
//            #!/bin/bash
//            export LC_ALL=C.UTF-8 
//            export LANG=C.UTF-8
//            pipenv install --three pytest pytest-html selenium
//            pipenv run pytest test_smoke.py  -v --junitxml="report-smoke.xml"
//            pipenv --rm
//            '''
//            perfReport modeThroughput: true, sourceDataFiles: 'report-smoke.xml'
//          }
//        }
//      }
    }
   }