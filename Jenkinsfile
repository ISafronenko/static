pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region: 'us-west-2', credentials: 'f9b54615-d006-481d-924a-74f2bcbc53c0') {
                    s3Upload(file: 'index.html', bucket: 'ievgen-udacity-pipeline')
                }
            }
        }
    }
}
