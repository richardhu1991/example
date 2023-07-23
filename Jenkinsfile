pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh '''wget -c https://dl.google.com/go/go1.20.6.linux-amd64.tar.gz
rm -rf /usr/local/go && tar -C /usr/local -xzf go1.20.6.linux-amd64.tar.gz
export PATH=$PATH:/usr/local/go/bin
pwd ls -al
go version'''
      }
    }

  }
}