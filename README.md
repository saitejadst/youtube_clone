# Build and Deploy a Modern YouTube Clone Application in React JS with Material UI 5
Project Overview of the 

Build and deploy a modern YouTube clone application using React Js, leveraging the Classic Editor and YAML. The project involves:

1. Creating a new project in Azure DevOps
2. Cloning the repository from (link unavailable) into Azure Repo
3. Setting up an Azure App Service to deploy the application
4. Defining build, run, and deployment steps using npm in the Classic Editor
5. Creating a pipeline using YAML code

Pipeline Steps:

1. Build: npm install and npm build
2. Run: npm start
3. Deploy: Azure App Service deployment

YAML Pipeline Code:

trigger:
- main

pool:
vmImage: 'ubuntu-latest'

steps:
- task: NpmInstall@1
- task: NpmBuild@1
- task: NpmStart@1
- task: AzureAppServiceDeploy@1

Please note that the above YAML code is a summary and you may need to add more tasks and configurations as per your requirements.

Here is a simplified explanation of the pipeline in 5 lines:

1.The pipeline builds the application using NPM install and run build commands.
2. The build artifacts are published to a container named "drop".
3.The pipeline deploys the application to an Azure Web App named "youtubeclone".
4.The deployment uses the build artifacts from the "drop" container and configures the web app with the necessary settings.

YAML File for project

https://github.com/saitejadst/youtube_clone/blob/main/YAML

SITE URL: https://youtube-staging-ahacc4h3ebapchcf.centralindia-01.azurewebsites.net/

DEPLOYING APPLICATION USING AZURE PIPELINE RELEASES

<img width="1522" height="705" alt="image" src="https://github.com/user-attachments/assets/524cdcac-2478-4b51-848f-de50c8db5069" />

