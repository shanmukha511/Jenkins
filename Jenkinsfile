	Pipeline
	{
	agent none
	stages
	 {
	stage('Build')
	 {
	 steps
	 {
	echo "Build Stage"
	sh "date"
	}
	 }
	stage('Test')
	  {
	  steps{
	echo "Test Stage"
	sh "whoami"
	  }
	  }
	stage('Deploy')
	 {
	 steps{
	echo "Deploy"
	sh "uname"
	 }
	 }
	}
	}
