pipeline {
  agent any
  stages {
    stage('Build&Package') {
      parallel {
        stage('Build&Package') {
          steps {
            echo 'Build&Package'
          }
        }
        stage('B2B') {
          steps {
            echo 'B2B Tests'
          }
        }
        stage('CE') {
          steps {
            echo 'CE Tests'
          }
        }
        stage('EE') {
          steps {
            echo 'EE Job'
          }
        }
      }
    }
    stage('Unit Tests') {
      parallel {
        stage('Unit Tests') {
          steps {
            echo 'Unit Tests'
          }
        }
        stage('CE') {
          steps {
            echo 'CE Unit Tests'
          }
        }
        stage('EE Unit Tests') {
          steps {
            echo 'EE Unit Tests'
          }
        }
      }
    }
    stage('Integration Tests') {
      parallel {
        stage('Integration Tests') {
          steps {
            echo 'Integration Tests'
          }
        }
        stage('CE') {
          steps {
            echo 'CE Integration'
          }
        }
      }
    }
    stage('Unit Code Coverage') {
      steps {
        echo 'Unit Code Coverage'
      }
    }
    stage('Feature UI Automation') {
      parallel {
        stage('Feature UI Automation') {
          steps {
            echo 'Feature UI Automation'
          }
        }
        stage('CE UI Automation') {
          steps {
            echo 'CE UI Automation'
          }
        }
        stage('EE UI Automation') {
          steps {
            echo 'EE UI Automation'
          }
        }
      }
    }
    stage('Feature Backend Automation') {
      steps {
        echo 'Feature Backend Automation'
      }
    }
    stage('Regression Tests') {
      parallel {
        stage('Regression Tests') {
          steps {
            echo 'Regression Tests'
          }
        }
        stage('CE Regression') {
          steps {
            echo 'CE Regression'
          }
        }
        stage('EE Regression') {
          steps {
            echo 'EE Regression'
          }
        }
      }
    }
    stage('Functional Automation Code Coverage') {
      steps {
        echo 'Functional Automation Code Coverage'
      }
    }
    stage('Smoke Tests') {
      steps {
        echo 'Smoke Tests'
      }
    }
    stage('Prod Monitoring Tests') {
      steps {
        echo 'Prod Monitoring Tests'
      }
    }
  }
}