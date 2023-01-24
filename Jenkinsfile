pipeline {
    agent any
    parameters {
        string(name: 'persona_a_saludar')
    }
    stages{
      stage('execution') {
          steps{
             js '/index.js'
          }
      }
    }
}  
