pipeline {
    agent any 
    stage('input') {
		try {
			timeout(time:10, unit:'SECONDS') {
				response = input message: 'User',
					parameters: [string(defaultValue: 'user1',
					description: 'Enter Userid:', name: 'userid')]
			}
		}
		catch (err) {
			response = 'user1'
		}
	}
}