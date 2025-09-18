pipeline {
    agent any

    triggers {
        pollSCM('H/5 * * * *')
    }

    stages {
        stage('Stage 1: Build') {
            steps {
                echo 'Task: Build the code'
                echo 'Tool: Maven'
            }
        }

        stage('Stage 2: Unit & Integration Tests') {
            steps {
                echo 'Task: Run unit & integration tests'
                echo 'Tool: JUnit'
            }
        }

        stage('Stage 3: Code Analysis') {
            steps {
                echo 'Task: Static code analysis'
                echo 'Tool: SonarCloud'
            }
        }

        stage('Stage 4: Security Scan') {
            steps {
                echo 'Task: Dependency vulnerability scan'
                echo 'Tool: OWASP Dependency-Check'
            }
        }

        stage('Stage 5: Deploy to Staging') {
            steps {
                echo 'Task: Deploy to staging'
                echo 'Tool: AWS EC2'
            }
        }

        stage('Stage 6: Integration Tests on Staging') {
            steps {
                echo 'Task: Run integration tests on staging'
                echo 'Tool: Selenium'
            }
        }

        stage('Stage 7: Deploy to Production') {
            steps {
                echo 'Task: Deploy to production'
                echo 'Tool: AWS EC2'
            }
        }
    }
}
