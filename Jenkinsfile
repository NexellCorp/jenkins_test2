pipeline {
  agent any
  stages {
    stage('print message') {
      steps {
        echo 'Nexell pipeline Start'
      }
    }
    stage('git pull') {
      steps {
        sh '''git pull abcde

'''
      }
    }
    stage('parent commit check') {
      steps {
        sh 'git cherry-pick abcd'
      }
    }
    stage('build') {
      steps {
        sh 'build.sh'
      }
    }
  }
}