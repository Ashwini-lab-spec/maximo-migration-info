Maximo Application Suite Readme File
### Introduction
This readme file provides information about the Maximo Application Suite project, its dependencies, and installation procedures.

### Prerequisites
Ensure you have the following prerequisites installed before proceeding:

Java Development Kit (JDK) 8 or later
Git version 2.25.0 or higher
Maven 3.x
### Installation
Follow these steps to install the Maximo Application Suite:

Clone the Maximo Application Suite repository:

git clone [External URL]

Navigate to the cloned repository folder:

cd maximo-application-suite

Build and deploy the Maximo Application Suite using Maven:

mvn clean package org.jenkins-ci.tools:maven-deploy-plugin:2.21:deploy

Access the Maximo Application Suite web interface by navigating to [External URL]

### Dependencies
The Maximo Application Suite depends on several external libraries. These dependencies are automatically managed by Maven.

### Building and Deploying the Maximo Application Suite
After installing the necessary tools and dependencies, you can build and deploy the Maximo Application Suite using Maven.

### Testing
To run the unit tests, navigate to the 
src/test/java
 directory and execute the following command:

bash mvn test

For integration testing, set up a database connection and execute the following commands:

Initialize the database schema: sql ./dbscripts/init_database.sh

Populate the database with sample data: sql ./dbscripts/populate_database.sh

Run the integration tests: bash mvn verify

### Troubleshooting
If you encounter any issues while working with the Maximo Application Suite, consult the troubleshooting section in the `src/main/resources

CIO CI / CD Pipeline Catalog

https://pages.github.ibm.com/cio-ci-cd/pipeline-catalog-docs
CIO CI / CD Pipeline Catalog

https://pages.github.ibm.com/cio-ci-cd/pipeline-catalog-docs/
Tasks - CIO CI / CD Pipeline Catalog

https://pages.github.ibm.com/cio-ci-cd/pipeline-catalog-docs/conventions/tasks/
Release Management - CIO CI / CD Pipeline Catalog

https://pages.github.ibm.com/cio-ci-cd/pipeline-catalog-docs/maintainers/release-management/
Requirements - CIO CI / CD Technical


### Maximo Migration Troubleshooting Guide
Introduction
This guide aims to assist users who are migrating their data from Maximo to another system. It includes common issues encountered during the migration process and solutions to resolve them.

### Prerequisites
Ensure you have completed the necessary prerequisites as outlined in the official Maximo migration guide provided by the vendor.

### Common Issues
Issue 1: Data Import Failure
When attempting to import data from Maximo, you may encounter an error related to invalid records.

### Solution
Check the integrity of the exported data file before importing it. Correct any errors identified and retry the import process.

### Issue 2: Connection Timeout Error
During the migration process, you might experience connection timeout errors while connecting to the Maximo database.

### Solution
Increase the connection time limit in your migration script or application settings. This can typically be done by modifying the 
connectTimeout
 parameter.

### Issue 3: Duplicate Records
After migrating data to the new system, duplicate records may appear due to mismatched primary keys.

### Solution
Update the primary key schema in both systems to ensure unique record identification. Implement a validation step in your migration script to prevent duplicates.

### Troubleshooting
If you cannot resolve the issue using the suggested solutions, refer to the official Maximo migration guide or contact the vendor's support team for assistance.

IBM Maximo Application Suite can already be deployed on AWS. However, if you're looking to migrate an existing installation of Maximo to AWS, there are several factors to consider. These include assessing your current environment, configuring networking and storage settings, migrating data and configurations, and testing the migrated system thoroughly. It's recommended to consult the official IBM Maximo Application Suite documentation and seek assistance from experienced professionals for a smooth transition.
