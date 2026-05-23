pipeline {
    agent any

    triggers {
        pollSCM('* * * * *')
    }

    stages {
        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Task: Build the code using a build automation tool to compile and package the application.'
                echo 'Tool: Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Task: Run unit tests and integration tests to verify the application functions as expected.'
                echo 'Tools: JUnit, TestNG'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Task: Analyse the code and ensure it meets industry standards.'
                echo 'Tool: SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Perform a security scan to identify vulnerabilities.'
                echo 'Tool: OWASP Dependency-Check'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploy the application to a staging server.'
                echo 'Tool: AWS CLI / AWS EC2'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Run integration tests in the staging environment.'
                echo 'Tool: Selenium'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploy the fully tested application to production.'
                echo 'Tool: AWS CLI / AWS EC2'
            }
        }
    }
}
