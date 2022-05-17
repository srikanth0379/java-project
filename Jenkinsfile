pipeline{
    agent {
        label "master"
    }
    stages{
        stage('Run for project'){
            steps{
                //sh "echo ${PROJECT_NAME}"
                script {
                    git url: "https://github.com/srikanth0379/java-project.git"
                    def BRANCH = sh(returnStdout: true, script: 'git rev-parse --abbrev-ref HEAD').trim()
                    echo "${BRANCH}"
                }
            }

        }
    }
}
