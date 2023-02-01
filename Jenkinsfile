pipeline {
    agent any
    parameters {
        string(name: 'parametro1')
        string(name: 'parametro2')
    }
    stages{
      stage('stage1') {
          steps{
             sh 'node /JenkinsScripts/script1 ${params.parametro1}'
            }
        }
        stage('stage2') {
          steps{
             sh 'node /JenkinsScripts/script2 ${params.parametro2}'
            }
        }
        stage('stage3') {
          steps{
             sh 'node /JenkinsScripts/script3 ${env.RESULTADO}'
            }
        }
      
    }
}  
