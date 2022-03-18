# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

In my Article CMS project, I use App Service:
- App Service saving cost than VM. App Service can be scalability ease. About availability I think it same. And a workflow, I can use CI/CD to deploy from github to App Service instead of deploying manually. Besides in VM I need to install environment for Python but in App Service I just need to choose the right environment instead of having to install
- App Service have:
    + Easy to chosse invironment (Python, C#, ...) instead of having to install
    + Integrate with DevOps (CI/CD to deploy, CLI, ...)
    + Can scale up or scale down maunal or automative when server overload
    + Have higher availability
    + More security with azure (Have AzureAD, easy to manager IP)
    + Manager log
    + Server less
    + Lower tier is F1: free
    + Can change configulation in azure
- Virtual Machine have:
    + Can install many application
    + Hard to deploy, hard to config environment (CORS, SSL, Security, ...)
    + Cannot automation scale
    + Avalability depends on the regions environment
    + Remote server to trace log
    + Lower tier is B1s: more than 7 dollars a month

- So I use App Service for this project because:

- App Service saving cost than VM (F1 is free but B1s 7$/month). App Service can be scalability ease than VMs. And a workflow, I can use CI/CD to deploy from github to App Service instead of deploying manually. Besides in App Service I just need to choose the right environment instead of having to install and config on VMs

### Assess app changes that would change your decision.

- In Virtual Machine, I think it have a log monitor to see the app loging. After that, It will be ok if it have some image environment (windows server with Python, windows server with .NET6, etc), it very convenient to run the app in Virtual Machine instead of install all environment, it take more time and may be have some issue. The last I thing disk in Virtual Machine can connect to Storage Account, it will be easier to manager file on it.

### My Python App Service.
- URL to my Python App Service: https://articlecmsas.azurewebsites.net/