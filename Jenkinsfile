pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Checkout the code
                git 'https://github.com/visweswars/flutter_chat_application.git'
                
                // Build Flutter app
                nohup 'flutter clean'
                nohup'flutter pub get'
                nohup 'flutter build apk' // or 'flutter build ios' for iOS
            }
        }
    }
}
