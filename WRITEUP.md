# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 



*Analyze costs, scalability, availability, and workflow:*
- VM is coming with low up-front cost 
- VM is more expensive than App Service but we can shut down when no need in use and to money consuming but with App Service we always pay even if not using.
- VM can be grouped for higher scalability, availability while App Service is good support at Vertial Scaling and Horizontal Scaling
- About workflow
  - Virtual Machine: When we need to deploy our app to VM I will talk about VM with Linux first step we need to use secure copy to copy our application to VM and then config the NGINX server redirect any request access from VM public IP to our application
  - With Azure App Service we only need to choose the runtime language like Python,.NET, Java,... and choose the repository of our application we focus on the application and Azure will handle the Infra.


*Choose the solution: According to me, I would choose the Azure App Service for this application's deployment for the following reasons:*
1. This application has only a few basic functions, and we don't have a need for a high-performance compute service, so we can consider it a light-weight app. In this situation, we can choose the App Service.
2. This application is small, so we head to setup this as fast as we can. At this point, App Service is still faster than Virtual Machine because we don't need to take time to first setup Virtual Machine.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

