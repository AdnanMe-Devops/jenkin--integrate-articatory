# jenkin--integrate-articatory
Create Jenkins CICD Pipeline with Artifactory Integration for Build Artifact Management
Integrating Jenkins with Artifactory provides you with an automated platform for building and managing deployable artifacts (binaries).

 will launch a Jenkins and Artifactory CICD environment using Docker containers on a provided EC2 instance and will then configure a Jenkins build pipeline to build, compile, and package a sample Java servlet web application. The build pipeline will publish the build artifacts into Artifactory, which in turn will catalog and register them.


Objectives


Install and configure a Jenkins and Artifactory CICD environment using Docker containers
Configure Jenkins with the Gradle plugin to perform the core build and packaging for a sample Java servlet web application
Configure Jenkins with the Artifactory plugin for automated build artifact management
Create and set up a Jenkins build pipeline using a Jenkinsfile hosted within a GitHub repo
Use the Artifactory web application to examine and review the registered and published build artifacts


step

A single EC2 instance, named cicd.platform.instance, which will have a public IP address attached


SSHing into the EC2 instance, named cicd.platform.instance
Use Docker Compose to launch the following Docker containers:
Jenkins
Artifactory
Using a browser, administer and configure Jenkins - installing the required plugins. Connectivity to Jenkins will be done via the cicd.platform.instance Public IP address 
Using a browser, administer and configure Artifactory. Connectivity to Artifactory will be done via the cicd.platform.instance Public IP address 
Create a Jenkins build pipeline and configure it to build a sample Java servlet web application hosted on GitHub, with the build artifacts being automatically published into Artifactory
Execute the Jenkins build pipeline and confirm that it has completed successfully, publishing the build artifacts automatically into Artifactory
Confirm that Artifactory has received and cataloged the Jenkins build artifacts
