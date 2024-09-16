How to install & Run on client side

Install Maven (https://maven.apache.org/install.html)
image

Deploying as a .jar

Open up a terminal (Powershell or Command) and "cd" to your my-app directory within your code base.

Run mvn clean package -Pproduction in the my-app directory (You need maven for this)

image

Move the temprecorder-1.0-SNAPSHOT.jar file in tempRecorder2\my-app\target to your desired location

Open up a terminal in the directory containing the jar file and run the command java -jar temprecorder-1.0-SNAPSHOT.jar (Make sure you don’t have any ports open on whatever port you set up the project to use in the application.properties file.) The app should be running at http://localhost:8080/login

image

Still need to Accomplish:

Get Metrics Page to load
Admin page needs to show and print out logging
When creating account, need to verify via email (or other)
Add a captcha for account creation
Apply a server host for the web app (Supports Java, such as an apache variety)
Added security for passing information, disabling development tools, etc
Color coding elements outside of nominal range for input temps (red=too hot, blue = too cold)
Protect Main Branch on Github
Change the database to a type that is persistent between runs, remains secure, and has as low of an install requirement as possible for the client and server.
Admin view needs to add the ability to change username, and clean up junk code left over from cloning Home page
When Ready to Deploy:

https://hostingtutorials.dev/blog/free-spring-boot-host-with-render

or try:

Heroku

Render

DigitalOcean App Platform

Platform Sh

Google App Engine

Azure App Service

Netlify

AWS Elastic Beanstalk

Red Hat OpenShift

Engine Yard

Firebase
