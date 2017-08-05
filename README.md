# gradledemo

## Step1:

Install gradle latest version.
Set env varibale GRADLE_HOME to gradle install parth. Example GRADLE_HOME = D:\Softwares\gradle-4.0.2
Set or update your Path variable to %PATH%D:\Softwares\gradle-4.0.2\bin;

## Step2:

Checkout the project and go to project home path
 
gradle taksk - this commad runs all the tasks defined in the build.gradle file

gradle build - build's the project

gradle run - build and runs the application.

##step3:
### build.gradle 

#### gradle runs based on plugin's. application plug in for building and running java applications. 
apply plugin : 'application'

#### Sets the src directory as source directory
sourceSets.main.java.srcDirs = ['src']


#### defining repository
repositories {
	mavenCentral()
}

#### Defining dependencies
dependencies {
	compile "joda-time:joda-time:2.2"
}

#### set main java program to start the application
mainClassName = 'com.demo.GradleDemo'


### How to Run application with out gradle installation
Gradle wrapper is used to run the application with out having gradle on local system.
Run below
#### gradle wrapper
#### gradlew build
#### gradle run
