## Application Launcher ##

Managing, configuring standalone java applications made easy with __Application Launcher__


### FEATURES ###

---

* Pre bundled script which would allow you to manage application instance in different environments seamlessly
* Configurations can be changed/added very easily
* Scripts supports init.d configuration and Windows Service modes
* Upgrading Application is just a matter of replacing libraries in lib folder
* you can added other jar files easily in the class path
* _application parameters_ and _jmv parameters_ can configured very easily


### Usage ###
After downloading the zip file copy your application and dependent jar files to RUNNER_HOME/lib
Modify line number 35 to add class containing main method
````
wrapper.app.parameter.1=com.your.MainClass
````
based on your environment start the appropriate script, you are done.

Application Launcher is based on [Java Service Wrapper][jswId]
![Java Service Wrapper][jswImageId]


### DIRECTORY DETAILS ###

---


* __data__ ==> contains files required for application, configuration etc

* __logs__ ==> this where launcher will spit out logs

* __conf__ ==> configuration that should be done to launcher is driven through files in this folder

* __lib__ ==> this folder contains __wrapper.jar__ and __*.jar__, and any other jars you want to make available to classpath

* __bin__ ==> binary executables are present here, based on you environment you have to execute one of the files in this directory



### FAQ ###
---



  [runnerImageId]: http://raw.github.com/mnadeem/JenkinsRunner/master/jenkins_logo.png  "Jenkins Runner"
  [jswId]: http://wrapper.tanukisoftware.com/  "Java Service Wrapper"
  [jswImageId]: http://wrapper.static.tanukisoftware.co.jp/images/jsw-logo.jpg "Java Service Wrapper"
