@Library('sharedlibsintelipost')_
pipeline {
    agent {label 'master'}
    
    stages {
        stage('Prepare sharedlibsintelipost') {
            steps {
                intelipostSetup(this)
            }
        } 
        stage ('Compile Stage') {
            

            steps {
               
                    mavenTest()  
                
            }
        }
        // stage ('Testing Stage') {

        //     steps {
        //         withMaven(maven : 'apache-maven-3.6.1') {
        //             sh 'mvn test'
        //         }
        //     }
        // }
        // stage ('Install Stage') {
        //     steps {
        //         withMaven(maven : 'apache-maven-3.6.1') {
        //             sh 'mvn install'
        //         }
        //     }
        // }
    }
}

