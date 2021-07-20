// USE THE CORRECT LIBRARY TO BUILD FROM. FOR A TAGGED VERSION TO BE BUILD USE THE CORRESPONDING VERSION of shared library.

pipeline {
    agent any

    environment {       
        GIT_BRANCH = utility.get_git_branch_edited(env.BRANCH_NAME) 
    } 
    stages
    {
        stage('test')
        {
            steps
            {
                echo "hello world"
            }
        }
    }
    
}

   
