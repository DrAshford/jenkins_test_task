pipeline {
        agent any

        stages {
                stage('Jenkins-build-step') {
                        steps {
                                sh 'echo "Hello another one!" > textfile.txt'
                        }
                }
        }

        post {
                always {
                        archiveArtifacts artifacts: 'textfile.txt', fingerprint: true
                }
        }
}
