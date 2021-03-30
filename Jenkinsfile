pipeline{
        agent any
        environment{
            DB_PASSWORD='root'
        }
        stages{
            stage('Run App'){
                steps{
                    sh "sudo docker-compose pull && sudo -E DB_PASSWORD=${DB_PASSWORD} docker-compose up -d"
                }

            }
        }    
}
