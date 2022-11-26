pipeline {
        agent any

        stages {
                stage('Jenkins-build-step') {
                        steps {
                                sh 'echo "Bye bye another one!" > textfile.txt'
                        }
                }
        }

        post {
                always {
                        archiveArtifacts artifacts: 'textfile.txt', fingerprint: true
                }
        }
}
