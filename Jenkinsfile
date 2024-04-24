pipeline {
  agent any
  stages{
    stage("Build & Test"){
      when {
        branch 'develop'
      }
      steps {
        echo "Building & Testing Application."
      }
    }
    stage("Dev Deploy"){
      when {
        branch 'develop'
      }
      steps {
        echo "Deploy to deve environment"
      }
    }
    stage("Test Deploy"){
      when {
        branch 'test'
      }
      steps {
        echo "Deploy to test environment"
      }
    }
    stage("Prod Deploy"){
      when {
        branch 'main'
      }
      steps {
        echo "Deploy to production environment"
      }
    }
  }
}
