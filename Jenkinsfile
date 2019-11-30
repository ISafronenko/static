pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region: 'us-west-2', credentials: 'AKIA22XC3QMLPXNO4XEV') {
                    s3Upload(file: 'index.html', bucket: 'ievgen-udacity-pipeline')
                }
            }
        }
    }
}
