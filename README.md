## Application Launcher ##

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


#### How do I change the port? ####

_Modify the JenkinsRunnder/conf/wrapper.conf file (line number 31) as follows_

	wrapper.app.parameter.2=--httpPort=8070



  [runnerImageId]: http://raw.github.com/mnadeem/JenkinsRunner/master/jenkins_logo.png  "Jenkins Runner"
  [jswId]: http://wrapper.tanukisoftware.com/  "Java Service Wrapper"
  [jswImageId]: http://wrapper.static.tanukisoftware.co.jp/images/jsw-logo.jpg "Java Service Wrapper"