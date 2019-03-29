# Migrate-Bitbucket-to-Git

repository bitbucket
https://bitbucket.io/projects/repository/ 

repository git
https://git.com/repository


Clone source repository
	https://user@bitbucket.io/repository/repo.git
	
Repository target
	https://git.com/repository/repo.git

Migrate
	
	Two ways to perform migration:

		First Form
		
			Open git bash
			Go to the folder in which we want to perform the cloning of the repository
				/c/Users//Desktop/
			Clone the bitbucket repositories to the local team
				git clone --recursive https://user@bitbucket.io/repository/repo.git
			Navigate to the repository folder
				cd repo
			We create a personal token to upload the code
				cf3ed5482fc2714fefdfsdfueuejejeekekqdbuwqdoqwndf356625c29f8b11414a8ee
			We upload every bitbucket project to git
				git remote add upstream https://user:cf3ed5482fc2714fefdfsdfueuejejeekekqdbuwqdoqwndf356625c29f8b11414a8ee@git.com/repository/repo.git
			We push the files
				git push upstream master
				
		Second Form
		
			Open git bash
			Go to the folder in which we want to perform the cloning of the repository
				/c/Users//Desktop/
			Clone the bitbucket repositories to the local team
				git clone --mirror https://user@bitbucket.io/repository/repo.git
			Navigate to the repository folder
				cd repo.git
			We create a personal token to upload the code
				cf3ed5482fc2714fefdfsdfueuejejeekekqdbuwqdoqwndf356625c29f8b11414a8ee
			We upload every bitbucket project to git
				git remote set-url --push origin https://user:cf3ed5482fc2714fefdfsdfueuejejeekekqdbuwqdoqwndf356625c29f8b11414a8ee@git.com/repository/repo.git
			We push the files
				git push --mirror
			

		
		


			
	



