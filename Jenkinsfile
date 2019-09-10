pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps {
           sh "export AWS_DEFAULT_REGION=us-east-1"
           sh "aws cloudformation validate-template --template-body file://bote3.json"
           sh "aws cloudformation create-stack --stack-name mystack-1 --template-body file://bote3.json --region 'us-east-1'"
            }
        }
    }
}