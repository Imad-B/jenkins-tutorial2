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
        }
}
