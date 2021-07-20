// USE THE CORRECT LIBRARY TO BUILD FROM. FOR A TAGGED VERSION TO BE BUILD USE THE CORRESPONDING VERSION of shared library.

pipeline {
    agent { label 'none' }

    environment {       
        GIT_BRANCH = utility.get_git_branch_edited(env.BRANCH_NAME) 
    }

    options {
        buildDiscarder(logRotator(numToKeepStr:env.NUM_OLD_BUILDS))
    }

    stages {
        stage('CheckNode') {
            steps {
                isUnix()
            }
        }
    	
        stage('View env variables') {
            steps {
                script {
                    sh """
                        echo $GIT_BRANCH
                    """
                }
            }
        }
        
        
    }
  }
