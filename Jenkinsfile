pipeline{
  agent any
  stages{
    stage("Build"){
      steps{
        echo "Building in progress"
        sh'''
        pip3 install -r requirements.txt
        '''
      }
    }
    stage("Test"){
      steps{
        echo "Testing in progress"
        sh'''
        python3 hello1.py
        '''
      }
    }
    stage("Deploy"){
      steps{
        echo "Deployment in progress"
        sh'''
        python3 hello2.py
        '''
      }
    }
  }
}
