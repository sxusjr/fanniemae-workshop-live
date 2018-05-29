pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo 'Hello World!'
        sh 'java -version'
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
      }
    }
  }
  environment {
    MY_NAME = 'Shehzad'
    TEST_USER = credentials('test-user')
  }
  parameters {
    string(name: 'Shehzad', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}