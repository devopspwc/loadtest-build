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
      stage('Build') {
        steps {
          dir ("${_DIR}") {
           sh label: '', script: '''
               gatsby build'''
          }
        }
      }
    }
   }