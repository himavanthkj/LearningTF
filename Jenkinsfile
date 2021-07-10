pipeline {
    agent any
    tools {
        terraform 'TerraformIAC'
    }
    stages {
        stage('Run Terraform') {
            steps {
                sh 'terraform init'
                sh 'terraform apply --auto-approve'
            }
        }
    }
}

