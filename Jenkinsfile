pipeline{
        agent any
        stages{
            stage('Make Directory'){
                steps{
                    sh "mkdir ~/jenkins-tutorial"
                }
            }
            stage('Make Files'){
                steps{
                    sh "touch ~/jenkins-tutorial/file1 ~/jenkins-tutorial/file2"
                }
            }
            stage('Clone Files'){
                steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Imad-B/jenkins-tutorial2.git']]])
                }
            }
        }
}

