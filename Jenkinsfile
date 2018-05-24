node {
    stage 'checkout'
    echo 'Checking out source code'
    git url: 'https://github.com/karthick87/jenkinsdemo'
    stage 'compile'
    echo "compile"
    sh "/opt/apache-maven/bin/mvn compile"
    stage 'test'
    echo "Test"
    sh "/opt/apache-maven/bin/mvn test"
}
