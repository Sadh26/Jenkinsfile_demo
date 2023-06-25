pipeline {
  agent any
  stages {
    stage('Package 1') {
      steps {
        git(url: 'https://github.com/Sadh26/LabviewJenkinsExample.git', branch: 'master')
        bat '.\\\\Scripts\\\\Build.bat'
      }
    }

    stage('Package 2') {
      steps {
        git(url: 'https://github.com/Sadh26/Jenkins_Demo.git', branch: 'master')
      }
    }

    stage('Final Step') {
      steps {
        echo 'This message  shouldn\'t be Displayed'
      }
    }

  }
}
