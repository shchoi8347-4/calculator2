pipeline {
     agent any
     stages {
          stage("Checkout") {
               steps {
                    git url: 'https://github.com/shchoi8347-4/calculator.git', branch: 'main'
               }
          }
          stage("Compile") {
                steps {
                    sh "./gradlew compileJava"
                }
          }
          stage("Unit test") {
                steps {
                    sh "./gradlew test"
                }
          }
    }
}