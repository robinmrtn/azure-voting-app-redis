pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                echo "$GIT_BRANCH"
            }
        }
        stage('Docker Build') {
            steps {
                powershell 'Write-Output "docker images -a"'
//                  pwsh 'docker images -a'
//                 pwsh """
//                 cd azure-vote/
//                 docker iamges -a
//                 docker build -t jenkins pipeline .
//                 docker images -a
//                 cd ..
//                 """
            }
        }
    }
}
