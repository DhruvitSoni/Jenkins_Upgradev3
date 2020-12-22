pipeline {
      agent any
      stages {
            stage('Init') {
                  steps {
                        echo 'We are Starting the Testing'
                  }
            }
            stage('Checkout SCM') {
                  git branch: 'dependabot/maven/java-tomcat-sample/junit-junit-4.13.1', credentialsId: 'dhruvitsoni', url: "https://github.com/DhruvitSoni/Jenkins_Upgradev3.git"
            }
            stage('Build') {
                  steps {
                        echo 'Building Sample Maven Project'
                  }
            }
            stage('Deploy') {
                  steps {
                        echo "Deploying in Staging Area"
                  }
            }
            stage('Deploy Production') {
                  steps {
                        echo "Deploying in Production Area"
                  }
             
            }
      }
}
