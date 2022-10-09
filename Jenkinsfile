pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                echo 'Build'
                sh 'mvn clean package'
            }
        }
            stage('Test'){
                steps{
                echo 'Test'
                sh 'mvn test'
            }
        }       
            stage('Sonarqube'){
                steps{
                    echo 'Sonarqube'
                }
            }
            stage('Push to Artifactory'){
                steps{
                    echo 'Push to Artifactory'
                }
            }
            stage('Deploy to Dev'){
                steps{
                    echo 'Deploy to Dev'
                }
            }
            stage('Deploy to QA'){
                steps{
                    echo 'Deploy to QA'
                }
            }
            stage('Deploy to UAT'){
                steps{
                    echo 'Deploy to UAT'
                }
            }
            stage('Deploy to Staging'){
                steps{
                    echo 'Deploy to Staging'
                }
            }
            stage('Deploy To Prod'){
                steps{
                    echo 'Deploy to Prod'
                }

            }
            post{
                failure{
                    echo 'Failed'
                }
                success{
                    echo 'Success'
                }
                always{
                    echo 'Always'
                }
            }
        
        }
    }
}