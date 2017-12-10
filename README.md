master-minds
============

### Local VM Database Popuation

The first step that needs to be done to set up the project so that it runs properly in the class VM is to populate the database.  Scripts have been created to automate this process, and can be run from a shell command prompt.  First, 'cd' into the 'database' subdirectory provided as part of the project build.  Then, to populate the database in your own virtual environment, do the following:

	To create all objects execute the following script:

	prompt:> runme_create_all.sh


	To drop all objects and clean out the database (for re-population of the database):

	prompt:> runme_drop_all.sh



If you want to execute individual scripts inside this directory each '.sql' file will also load into the database on its own.  
Just follow the example in one of the 'runme' scripts to see how to log into MySQL and execute a script.  You can also log in 
as follows:

	prompt:> mysql -u root -proot

	mysql> source <filename.sql>






------------------------------------------------------------------------

Implementation of the dynamic course allocation system

Steps to get the project up and running on local :-

Step 0:-

Clone the repository into your local using the command:-
git clone https://github.gatech.edu/ssrivastava64/master-minds.git

Step 1:-

Install Eclipse (if not already installed) using the link below :-
https://eclipse.org/downloads/packages/eclipse-ide-java-ee-developers/lunasr2

Run eclipse and then in the left hand side "Project Explorer" tab right click and select import and import the project from the directory where the git repository was cloned.
        
Step 2:-

Download and install apache tomcat version 8.0.
Download using the link:- 
https://tomcat.apache.org/download-80.cgi
Install apache tomcat in eclipse using:-
http://www.coreservlets.com/Apache-Tomcat-Tutorial/tomcat-7-with-eclipse.html

Step 3:-

Select the servers tab and then right click on the server and select add/remove project. Add the imported project into the server.

Step 4:-

Start the server. Check the console to see the following message "INFO: Server startup in 8555 ms". Once the server has started up the home page can be accessed by using the following url:
http://localhost:8080/Project4/

A welcome page should display.

Step 5:-
Click on Welcome to navigate to the login page. The user id and password currently being used is admin/123456. Entering a wrong userid/pwd will display an error. To access the admin page use the url 
http://localhost:8080/Project4/admin 
and use the same user id/pwd :
admin/123456 
to access the admin page. 
A page with a logout option will be displayed. Clicking on the logout logs you out of the application and displays the login page again.





         
