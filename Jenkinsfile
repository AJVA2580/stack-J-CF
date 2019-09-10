pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps {
           sh "export AWS_DEFAULT_REGION=us-east-1"
           sh "aws cloudformation create-stack --stack-name mystack --template-body file://bote3.yaml --region 'us-east-1'"

            }
        }
    }
}