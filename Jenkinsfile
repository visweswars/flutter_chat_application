pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Checkout the code
                git 'https://github.com/visweswars/flutter_chat_application.git'
                
                // Build Flutter app
                sh 'flutter clean'
                sh'flutter pub get'
                sh 'flutter build apk' // or 'flutter build ios' for iOS
            }
        }
    }
}
