# Task create a CI/CD pipeline and supporting infrastructure from scratch on Azure

Task is to automate the deployment and provisioning of resources that host the app provided. 
It should be hosted in a highly available and scalable web application hosted in Azure.

Link to the site that has been deployed [here](https://devopsinterview.azurewebsites.net/)

For source code please refer [here](https://github.com/singuvenkatesh/devops-interview)

### Pre-requsites
- Below are the pre-requsites for this project.
    -  Create a Azure free account [Azure portal](https://portal.azure.com/)
    -  Azure Devops account [Azure Devops portal](https://dev.azure.com/)
    -  Github account for storing the source code [github](https://github.com/singuvenkatesh/devops-interview)
    -  Agent pool setup for windows on azure devops
    -  .NET Core sdk 3.1.415 is to be installed on Agent pool
    -  IAC for provisioning of resources using Terraform
    -  Service principle connection setup
    -  create a free account with [AccuWeather](https://developer.accuweather.com/) in order to register an application and call their API

### AccWeather CI/CD Process
 ![Alt text](screenshots/accweather_cicd_process.jpg?raw=true "Optional Title")
  
### Setup CI/CD pipeline DevOps project
- Created a build and release pipelines to compile, test and deploy the application and now ready to collaborate with a team on an ASP.NET Core app with a CI/CD process that automatically deploys your latest work to your web site.
    - Infrastructure provisioning of following resources 
         ```
                1.1 Resource group
                1.2 App Service Plan
                1.3 App Service
                1.4 Storage account
                1.5 storage container 
         ```
       source code is available here ![infra](infrastructure) 
         
    - automating the build and deploying the application
        
        source code is available here ![pipelines](pipelines)
        
    - Update existing code in order to add API key in the below files 
        
        ![API key](Src/Presentation/BradyWeather.Blazor.Server/appsettings.Development.json)
        
        ![API key](Src/Presentation/BradyWeather.Blazor.Server/appsettings.json)
        
  ### At the end of the exercise the application should look like below
        
     ![Alt text](screenshots/app_screenshot.png?raw=true "Optional Title")
     
     
     
  ### Advantages of this soultion is easy to scale and maintain. This soultion is always highly avaiable.
      
    
       
