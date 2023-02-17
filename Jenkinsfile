pipeline {
 agent any
 stages {
 stage('Build') {
 steps {
 sh 'g++ -o PES2UG20CS388-1 ./main/hello.cpp'
 echo 'BuildiNG it successful'
 }
 }
 stage('Test') {
 steps {
 sh './PES2UG20CS388-1'
 echo 'Testing  it successful'
 }
 }
 stage('Deploy') {
 steps {
 echo 'Deploying it successful'
 }
 }
 }
 post {
 failure {
 echo 'Pipeline has failed'
 }
 }
}
