pipeline {
    agent none
    stages{
        stage('build') {
            agent none
            step{
                echo "test"
            }  
        }
       stage ('Deploy') {
             agent none
             step{
                   sshagent(credentials : ['b0543eb0-0242-41e7-8e34-044591cf6a33']) {
                   sh 'python --version'
                   }
                 }
       }
    }
}
