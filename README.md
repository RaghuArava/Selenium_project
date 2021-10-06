# Selenium_project
Editer:Pycharm
languages:python
Framwork:Behavior Driven Development with behave (it is popular with java + cucumber + gherkin )
 
Note:Unzip the zip folder(Folder structure will not be effected)

Prerquisetes:
1.python3 should be installed.
2.pycharm should be installed.
3.install the below mentioned packages from the pycharm
	a>selenium package
	b>behave (BDD) tool package
	c>requests package

How to install the packages on pycharm?
	-> Select the Project located at left and Go to 'File' -> Settings -> Project -> Python Interpreter
		click on + symbol located at top left or right(dependes on pycharm version) type the required packages and click install
		make sure python interpreter configured with /path/to/python.exe

Project structure:
	<Project Folder> 
		features folder
			steps folder
				testcases file1.py
				testcases file2.py	
			feature file1.feature
			feature file2.feature

Note:feature file name should have extension <.feature> ,Ex:file.feature. (Here pycharm will notify to install feature plugin)
			
How run the secnarios?
	1.Go to project folder on pycharm(Here you will see features folder)
	2.Click on terminal (mostly located at left bottom)
	3.Run the feature file with behave 
		Ex:behave featurers/featureFile.feature

How to run the current project?
	1.Go to the project name 'Bahave' on pycharm
	2.To run the Backend test scenario's, run the below command 
		 behave .\features\cryptoCurencyFrontEndVerification.feature   (We should be located at Behave folder)
	3.To run the Frontend test scenario's, run the below command
		 behave .\features\cryptoCurencyFrontEndVerification.feature

Note: by defauld std.output will not be resulted since it will be suppressed by behave,inorder to get it we need keep the behave.ini with following content
	Behave\features\behave.ini
		[behave]
		stderr_capture=False
		stdout_capture=False

	 
		  
