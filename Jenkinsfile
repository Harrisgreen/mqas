pipeline {
    agent any
    stages {
		stage('run-parallel-branches') {
			steps {
				parallel(
					a: {
						echo "This is branch a"
					},
					b: {
						echo "This is branch b"
					}
				)
			}
		}
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
    }
}
