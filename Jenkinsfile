node {
    def MAVEN_HOME = tool "mymaven1"
    env.PATH = "${env.PATH}:${MAVEN_HOME}/bin"
    
    
    stage('Checkout') {
        checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/ved2728/credit-service.git']]])
    }
        stage('Inital Setup'){
            sh 'mvn clean compile'
        }
    stage ('unit testing'){
        sh 'mvn test'

    }
    
}
