# Weather forecast API app with database deployed as Azure App service and Azure SQL database
This solution is a .NET 9 Web API that interacts with a SQL Server database to manage and retrieve weather data. The backend is built using Minimal APIs, providing a concise and efficient architecture for building HTTP services. The database is implemented using a code-first approach with Entity Framework Core, allowing the schema to be generated and updated through migrations.

## Azure Deployment with Publish Profile
The solution includes a publish profile designed to automate the deployment of the application to Microsoft Azure. This profile handles the provisioning and configuration of two key Azure resources:

1. Azure App Service
   * Hosts the Web API.
   * Provides a scalable, managed environment for deploying and running the application.
   * The publish profile includes settings for build configuration, deployment mode, and resource targeting.
  
2. Azure SQL Database
     * Serves as the cloud-hosted relational database backend.
     * Automatically configured to work with the deployed Web API.
     * Connection strings and related settings are managed via app settings in the App Service.
  
By using the publish profile, the deployment process becomes seamless—developers can deploy directly from Visual Studio or the command line with minimal configuration, ensuring consistency between development and production environments.
