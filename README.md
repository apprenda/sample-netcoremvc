# Sample .NET Core MVC Application with docker
Sample .NET Core MVC Application with docker for deployment to Apprenda

The repository contains basic .NET Core MVC template provided by Microsoft with the addition of a Dockerfile for packaging in a docker container. Additionally, an Apprenda archive is provided if you wish to deploy to an Apprenda environment with docker enabled. 

There are two options to follow in order to deploy in your environment:
1. Deploy the already provided and built docker container
2. Build the application and your own docker container for deployment

#Deploying Existing Container
1. Deploy the Archive.zip file to Apprenda as a new application. The file is provided within the archive folder in this repository.

#Build your Own Container
1. Navigate to the src directory of the repository
2. Run "dotnet publish" in order to build and publish your application files.
3. Build a docker container using the provided Dockerfile and push to your repository of choice.
4. Modify the DeploymentManifest file provided in the archive folder with the correct information (Image Name).
5. Zip the linuxServices and DeploymentManifest files to create an Apprenda Archive. 
6. Deploy to Apprenda.
