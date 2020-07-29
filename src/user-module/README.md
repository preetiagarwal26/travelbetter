# Getting started
This module contains REST APIs to manage user, user-activities. Thes instructions will get you a copy of the project up and running on your local machine for development and testing purposes

# Prerequisites
What things you need to install the software and how to install them

Install maven from https://maven.apache.org/install.html

Create account with IBM Cloud.

Install IBM CLI (Refer to https://cloud.ibm.com/docs/cli?topic=cli-getting-started#overview)

Provision a CouchDB instance using Cloudant (Refer to https://cloud.ibm.com/docs/Cloudant?topic=Cloudant-creating-an-ibm-cloudant-instance-on-ibm-cloud)

# Local Setup

Download this module

Modify /user-module/src/main/resources/application.properties with your Cloundant instance details

Navigate to user-module and perform **mvn clean install**

After clean build, run main class /user-module/src/main/java/com/callforcode/travelbetter/TravelBetterApplication.java

Access swagger using http://localhost:8080/swagger-ui.html

Built with
IBM Cloudant - The NoSQL database used
IBM CLI 
Maven - Dependency management
Springboot - Used to generate backend user , activity CRUD APIs
