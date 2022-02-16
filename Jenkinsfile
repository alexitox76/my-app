node{
    stage('SCM Checkout'){
        git 'https://github.com/alexitox76/my-app'
    }
    stage('Compile-Package'){
        //Get maven home path
        def mvnHome = tool name: 'Maven3', type: 'maven'
        sh "${mnvHome}/bin/mvn package"
    }
}