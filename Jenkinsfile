pipeline {
agent any
environment {
    JAVA_HOME="C:/zensar/jenkins-docker-training-dap/jdk-17.0.12_windows-x64_bin/jdk-17.0.12"
  }
stages {
stage('Clean stage') {
steps {
dir("StockApp") {
bat 'C:/zensar/jenkins-docker-training-dap/apache-maven-3.9.9-bin/apache-maven-3.9.9/bin/mvn clean'
}
}
}
 
stage('Compile stage') {
steps {
dir("StockApp") {
bat 'C:/zensar/jenkins-docker-training-dap/apache-maven-3.9.9-bin/apache-maven-3.9.9/bin/mvn compile'
}
}
}
 
stage('Install stage') {
steps {
dir("StockApp") {
bat 'C:/zensar/jenkins-docker-training-dap/apache-maven-3.9.9-bin/apache-maven-3.9.9/bin/mvn install'
}
}
}
 
}
}
