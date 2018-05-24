pipeline {
    agent any

    stages {
	stage ('Compile Stage') {
            steps {
		withMaven(maven : 'maven_3_5_3')' {
                    sh 'mvn clean compile'
                 }
            }
        }   

            
        stage ('Testing Stage') {
            steps {
                withMaven(maven : 'maven_3_5_3')' {
                    sh 'mvn test'
                }
            }
        }


        stage ('Packaging Stage') {
            steps {
                withMaven(maven : 'maven_3_5_3')' {
                    sh 'mvn test'
                 }
             }
        }

        stage ('Deploy Stage') {
            steps {
                withMaven(maven : 'maven_3_5_3')' {
                    sh 'mvn test'
                }
             }
        }
    }
}
 
