jenkins{
    agent any
    stages{
        stage('build'){
            steps{
                sh 'git clone https://github.com/rohit-nunam/hello-world-jenkins'
                sh 'mvn clean package'
            }
        }
        stage('Run'){
            steps{
                sh 'java -cp target/hello-world-1.0-SNAPSHOT.jar org.example.Main'
            }
        }
    }
}