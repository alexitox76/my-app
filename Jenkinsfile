node(){
    stage('SCM Checkout'){
        git 'https://github.com/alexitox76/my-app'
    }
    stage('Compile-Package'){
        //Get maven home path
        def mvnHome = tool name: 'Maven3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }
    stage('Email notification'){
        mail bcc: '', body: '''Hi sono Alessio, questa è una notifica di Jenkins.
        thanks
        Alessio''', cc: '', from: '', replyTo: '', subject: 'jenkins test', to: 'alexitox76@gmail.com'
    }
}
