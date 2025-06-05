pipeline {
agent any
tools {
gradle 'Gradle'
jdk 'JDK'
}
stages {
stage('Checkout') {
steps {
git branch:'master', url:'https://github.com/Harsheen23/gardle.git'
}
}
stage('Build') {
steps {
sh 'gradle build'
}
}
stage('Test') {
steps {
sh 'gradle build'
}}
stage('Run Application') {
steps{
sh 'gradle run'
}
}
}
post {
success {
echo 'Run successfully'
}

failure {
echo 'Run failed'
}
}
}

