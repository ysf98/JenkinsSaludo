pipeline {
    agent any
    triggers {
        cron('H/05 * * * *')
    }
    parameters {
        string(name: 'persona_a_saludar')
    }
    stages{
      stage('execution') {
          steps{
             sh 'node index'
            }
        }
      stage('Parallel') {
          parallel {
              stage('Parallel 1') {
                  steps {
                      echo "Hola mundo 1"
                    }
                }

              stage('Parallel 2') {
                  steps {
                      echo "Hola mundo 2"
                    }
                }
            }
        }
    }
}  
