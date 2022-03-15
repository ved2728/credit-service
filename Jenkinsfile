node {
    stage('Checkout') {
        checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/ved2728/credit-service.git']]])
    }
}
