tools { 
    maven 'maven_3_5_3' 
    jdk 'java_1_8' 
}

node {
    stage 'SCM Checkout'
    echo 'Checking out Source Code'
    git url: 'https://github.com/karthick87/jenkinsdemo'

    stage 'Build'
    echo "Starting clean compilation"
    sh "/opt/apache-maven/bin/mvn compile"

    stage 'Unit Test'
    echo "Running Test Cases"
    sh "/opt/apache-maven/bin/mvn test"

    stage 'Packaging'
    echo "Packaging the Application"
    sh "/opt/apache-maven/bin/mvn package"

    stage 'Publish'
    echo "Pushing it to Artifactory"
    sh "/opt/apache-maven/bin/mvn deploy"
}
