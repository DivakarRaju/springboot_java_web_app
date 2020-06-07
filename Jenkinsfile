node ('slave-1') {
    stage('Build') {
            git 'https://github.com/DivakarRaju/springboot_java_web_app.git'
            sh "mvn -Dmaven.test.skip=true package"
    }
}
node ('slave-2') {
    stage('Test') {
            git 'https://github.com/DivakarRaju/springboot_java_web_app.git'
            sh "mvn test"
    }
}