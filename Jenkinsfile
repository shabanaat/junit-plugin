pipeline {
    agent any
    stages {
        stage('Build') {
            when {
                allOf {
                    not { branch 'master' }
                    environment name: 'JOB_NAME', value: 'Foo'
                }
            }
            steps {
                echo 'Building'
            }
        }
    }
}
