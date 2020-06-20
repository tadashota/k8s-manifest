pipeline {
  agent {
    kubernetes {
      cloud 'openshift'
      yamlFile 'jenkins-agent-pod.yaml'
    }
  }

  stages {
    stage('test') {
      steps {
        sh '''id
        pwd
        ls
        oc whoami'''
      }
    }
  }
}
