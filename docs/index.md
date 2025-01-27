# Trusted Application Pipeline Software Template

This application, **pqb99qjcp-nodejs**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/rhtap-test-organization-jk/pqb99qjcp-nodejs ](https://github.com/rhtap-test-organization-jk/pqb99qjcp-nodejs ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/rhtap-test-organization-jk/pqb99qjcp-nodejs-gitops ](https://github.com/rhtap-test-organization-jk/pqb99qjcp-nodejs-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |   
| **rhtap-app-development** | The default application during development. Every build will be deployed to this namespace for testing. | 
| **rhtap-app-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/rhtap-test-organization-jk/pqb99qjcp-nodejs-gitops ) in the components/pqb99qjcp-nodejs/overlays/prod directory |  
| **rhtap-app-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/rhtap-test-organization-jk/pqb99qjcp-nodejs-gitops ) in the components/pqb99qjcp-nodejs/overlays/prod directory | 