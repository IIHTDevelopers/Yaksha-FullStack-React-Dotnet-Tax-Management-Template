BackEnd-Commands
* On command prompt, cd into your project folder (cd <Your-Project-folder>).

* To connect SQL  server from terminal:
(TaxManagement /sqlcmd -S localhost -U sa -P pass@word1)
	-To create database from terminal - 
	1> Create Database TaxDb
	2> Go

*	Steps to Apply Migration(Code first approach):
	- Press Ctrl+C to get back to command prompt
	- Run following command to apply migration-
             (TaxManagement /dotnet-ef database update)

* To check whether migrations are applied from terminal:
(TaxManagement /sqlcmd -S localhost -U sa -P pass@word1)

	1> Use TaxDb
	2> Go
	1> Select * From __EFMigrationsHistory
	2> Go

* To build your project use command:
	(TaxManagement /dotnet build)

* To launch your application, Run the following command to run the application:
	(TaxManagement /dotnet run)

* To test web-based applications on a browser, use the internal browser in the workspace. Click on the second last option on the left panel of IDE, you can find Browser Preview, where you can launch the application.
	Note: The application will not run in the local browser

* To run the test cases in CMD, Run the following command to test the application:
	(TaxManagement .Tests/dotnet test --logger "console;verbosity=detailed")
	(You can run this command multiple times to identify the test case status,and refactor code  to make maximum test cases passed before final submission)             
* You need to use CTRL+Shift+B - command compulsorily on code IDE, before final submission as well. This will push or save the updated contents in the internal git/repository, and will be used to evaluate the code quality.


FrontEnd-Commands
* You can follow series of command to setup React environment once you are in your project-name folder:

* Follow the steps below to install and use Node.js version 18.20.3 using nvm:
	- Install nvm:
		curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash

	- Set up nvm environment:
		export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")" && [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"

	-Verify nvm Installation:
		command -v nvm

	- Install Node.js Version 18.20.3:
		nvm install 18.20.3

	- Set the installed Node.js version as active:
		nvm use 18.20.3

* On command prompt, cd into your project folder (cd <Your-Project-folder>).

* npm install -> Will install all dependencies -> takes 10 to 15 min

* npm run start -> To compile and deploy the project in browser. You can press <Ctrl> key while clicking on localhost:8081 to open project in browser -> takes 2 to 3 min

* npm run jest -> to run all test cases and see the summary

* npm run test -> to run all test cases. It is mandatory to run this command before submission of workspace -> takes 5 to 6 min

* You need to use CTRL+Shift+B - command compulsorily on code IDE, before final submission as well. This will push or save the updated contents in the internal git/repository, and will be used to evaluate the code quality.
