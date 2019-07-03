# Selenium-Automation
Tools Used:
------
	- Eclipse 2019 06
	- Maven
	- Selenium 3.141.59 dependency in pom.xml
	- TextNG
	- Logging using log4j 2
	- Chrome driver version 75

Instructions to import and run the automation project:
-------------------------------------------
	- Open eclipse.
	- From File --> import --> Existing maven project.
	- Specifiy root directory press on finish.
	- Build the project, so it can download all required jars from repository (it will appear in maven dependencies).
	- Right click on the project Google-PlayStore and choose Build Path --> Configure build path.
	- Navigate to libraries tab.
	- Change the log4j file from existing directory to YourDIR\Google-PlayStore .
	- Then Press on Apply and Close (it should path updated under Referenced Libraries).
	- Open Config.propperties file under Google-PlayStore\src\main\java\Config-File
	- Edit value of driverPath with YourDIR\\Google-PlayStore\\src\\main\\resources\\chromedriver.exe
	- Clean the project.
	- Right click on testng.xml from menu Run As --> TestNG Suite

Notes:
------
	- Maven client need to be installed inside eclipse.
	- TestNG need to be installed in eclipse
	- In the root directory of the project there is a zip file for log4j.jar (along with the jar file itself), if it is became corrupted.
	- in Google-PlayStore\src\main\resources the chrome driver along with zip file for it, if it became corrupted.

Maven Installation: (below for old releases, current eclipse release 2019 06 has Maven already installed with it)
	- From menu help, choose install new software.
	- Press on Add
	- Type http://download.eclipse.org/technology/m2e/releases in the URL and M2Eclipse in the name then press on add
	- It will show TestNG in below menu, choose all of it parent and subs and accept the package to install TestNG.

TestNG Installtion: (below setup is the only working now, TestNG does not appear in marketplace currently)
	- From menu help, choose install new software.
	- Press on Add
	- Type http://beust.com/eclipse in the URL and TestNG in the name then press on add
	- It will show TestNG in below menu, choose all of it parent and subs and accept the package to install TestNG.
