pipeline {
    agent any
    parameters {
        string(persona_a_saludar: 'Juan')
    }
    stages{
      stage('execution') {
          steps{
             sh 'node index'
          }
      }
    }
}  