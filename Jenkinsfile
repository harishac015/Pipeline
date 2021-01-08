pipeline {
	agent any 
	stages {
		stage ('build') {
			steps {
				sh '''
						echo "this is build stage"
						sleep 2
				   '''	
			} 
		}
		Stage ('deploy') {
		parallel {
		stage ('deploy1') {
			steps {
				sh '''
						echo "this is deploy1 stage"
						sleep 2
				   '''	
			}	   
		}
		stage ('deploy2') {
			steps {
				sh '''
						echo "this is deploy2 stage"
						sleep 2
				   '''	
			}
                                 }
                  }
                                }	   
		stage ('test') {
			steps {
				sh '''
						echo "this is test stage"
						sleep 2
				   '''	
			}	   
		}
	}
}
