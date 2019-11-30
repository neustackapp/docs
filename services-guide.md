# Services Guide

> This is a detailed guide of managing the full life cycle of services.

## Create

Using NeuStack, you can create various types of serverless solutions through a simple "Create Service" option.

### API

Creating an API is a simple process. Once you login, follow the steps below:

* Click on Create Service
* `Type`: Select "API" here
* `Provider` - Select from the choices available. The options available are set by your admins.
* `Runtime` - Select the appropriate language runtime. The runtime options available are based on the Provider selected and what your admins have made available
* `Name` - Give a name to your service 
* `Team` - Select your project/team name
* `Description` - (Optional) Provide service description 
* Click `Submit`

Your `API` will be available shortly.

### Function

You can create different types of functions through a simple process. Once you login, follow the steps below:

* Click on Create Service
* `Type`: Select "Function" here
* `Provider` - Select from the choices available. The options available are set by your admins.
* `Runtime` - Select the appropriate language runtime. The runtime options available are based on the Provider selected and what your admins have made available
* `Name` - Give a name to your service 
* `Team` - Select your project/team name
* `Description` - (Optional) Provide service description 
* `Event Schedule` - If your intention is to create a function that runs on a schedule, select "Fixed Rate of" and provide the schedule. For more advanced options, you can select "Cron Expression" and provide the appropriate [cron expression](https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/ScheduledEvents.html#CronExpressions). 
* `Events` - You can choose one of the function triggers from the options provided. This option is available only if you haven't chosen an "Event Schedule"
* Click `Submit`

Your `Function` will be available shortly.

### Website

Create [Angular](https://angular.io/), [React](https://reactjs.org/), [Vue](https://vuejs.org/) and other SPA websites through a simple process. Once you login, follow the steps below:

* Click on Create Service
* `Type`: Select "Website" here
* `Provider` - Select from the choices available. The options available are set by your admins.
* `Framework` - Select the framework that you would like to use. The framework options available are set by your admins
* `Name` - Give a name to your service 
* `Team` - Select your project/team name
* `Description` - (Optional) Provide service description 
* Click `Submit`

Your `Website` will be available shortly.

## Build & Deploy

NeuStack comes with a built-in Continuous Integration/Continuous Deployment (CI/CD) platform so that your developers have one less thing to worry about. Once developers push changes to `origin`, NeuStack will detect the changes and start building as well as deploying your changes to the respective environment. 

## Environments
By default, NeuStack deploys any changes to `master` (merged PRs or direct push) to your production environment. 

When NeuStack detects a new branch is created on `origin`, it will build the source code in the new branch as well as create and deploy to a new environment. For any changes to a `non-master` branch, it builds and deploys the changes to only that environment, thereby keeping the environments isolated from other changes.

## Templates

NeuStack comes with best practices templates for the service types selected along with the run-time. 