pipeline{
        agent any
        stages{
            stage('Make Directory'){
                steps{
                    sh "mkdir ~/jenkins-tutorial3"
                }
            }
            stage('Make Files'){
                steps{
                    sh "touch ~/jenkins-tutorial3/file1 ~/jenkins-tutorial3/file2"
                }
            }
            stage('Clone Files'){
                steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Imad-B/jenkins-tutorial2.git']]])
                }
            }
        }
}

