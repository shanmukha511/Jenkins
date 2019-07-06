pipeline {
  environment {
   
    // this assumes that "cred1" has been created on Jenkins Credentials
    CRED1 = credentials("Unix Slave Cred1")
    INBETWEEN = "Something in between"
    // this assumes that "cred2" has been created in Jenkins Credentials
    
  }

  agent any

  stages {
    stage("foo") {
      steps {
        // environment variables are not masked
        sh 'echo "$CRED1_USR or $CRED1_PSW"'
      

        // credential variables will be masked in console log but not in archived file
        sh 'echo $CRED1 > cred1.txt'
        sh 'echo $CRED2 > cred2.txt'
        archive "**/*.txt"
      }
    }
  }
}
