pipeline {
    agent any
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
          parallel(
                a: {
                    echo "Hola 1"
                },
                b: {
                    echo "Hola 2"
                }
            )
        }
    }
}  
