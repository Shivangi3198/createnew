pipeline{
  agent any{
    stages {
      stages('One') {
        steps{
          echo 'HI , this is shivangi '
        }
      }
      stage('Two'){
        steps{
          input('Do you want to proceed')
        }
      }
      stage('Three'){
        when{
          not{
            branch "master"
          }
        }
        steps {
          echo "Hello"
        }
      }
    }
