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
        sh '''
        oc apply -f nginx-deployment.yaml'''
      }
    }
  }
}
