# Jenkinsfile

Purpose of this repository:

I developed an Ansible Role on my Mac to install and configure Tomcat on a server (my case on an EC2). 
Jenkins was used to run the Ansible role and was tested and wroking correctly.

Next step was to use the Jenkins supplied by the cloud inrastructure team at my work.

I happly configued this Jenkins to execute my Anisble role and it was faling spectacularly. I was stumpped !!

As this Jenkins was running on a Docker (on some cloud on far away Galaxy) I didnt have access to the underlying platform where Docker is being run to look at what was happening.

To understand what was happening I wrote this Jenkinsfile to interrogate the docker.

Modify and use as your requirements.  

Configuring Jenkins:  

New Item  
 Name of the project
 Select Pipeline

  Click 'Pipeline' Tab
    Definition = Pipeline script from SCM (From pull down menu)
    SCM = Git
    Repository URL = https://github.com/vmendis/Jenkinsfile.git
    Credentials - none
  Branches to build  */master
Script Path = Jenkinsfile
