# Mobile Sample for Bluemix
[![](https://img.shields.io/badge/bluemix-powered-blue.svg)](https://bluemix.net)

### IBM Mobile Sample OpenWhisk

The sample uses the following Bluemix compute and mobile services:

**Compute**
* **OpenWhisk** a cloud-first distributed event-based programming service

**Services**
* **Push Notifications** for sending notifications to customers

### Architecture
insert diagram

## Configuring the Sample

The sample can be easily installed using the **bluegen** command line tool. This CLI tool logs you into Bluemix and prepares the backend services for use. It automatically provisions the services and registers the OpenWhisk actions you need quickly.

### Before you begin
Ensure that you have:

* The [Cloud Foundry CLI tool](https://github.com/cloudfoundry/cli) installed
* The [Bluemix Generator CLI tool](https://www.npmjs.com/package/bluemix-generator) installed by typing the command:

	`npm install -g bluemix-generator`

### Create your sample from this template

1. First, clone this project into your working directory:

	`git clone https://github.com/ibm-bluemix-mobile-services/bms-samples-nodejs-openwhisk`

2. Run the following command in the root directory of your cloned project. This will create the required services on Bluemix:

	`bluegen`

3. Navigate to your newly created projects folder.
4. Upload your Express application to Bluemix by typing these commands:

	`cf login [-a API_URL] [-u USERNAME] [-o ORG] [-s SPACE]`

	`cf push`

   After running `cf push`, you should be able to see the application running on the Bluemix dashboard. Visiting the application route will greet you with a landing page displaying more information about this template and the ability to explore the API.

5. You can run the sample locally by typing the commands:

	`npm install`

	`npm start`

### License
This package contains sample code provided in source code form. The samples are licensed under the Apache License, Version 2.0 (the "License"). You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0 and may also view the license in the license file within this package.
