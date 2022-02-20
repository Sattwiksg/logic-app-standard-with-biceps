# logic-app-standard-with-biceps
Logic App Standard workflow with biceps deployment

## Infrastructure & Components to reuse
This code expects following components to be already in place as part of available infrastructure
- A Resource Group
- An APIM Instance
- Any Frontdoor configuration (In case frontdoor is used before APIM)
- VNET and SUBNET configured
- ASEv3 instance available where this solution can be deployed
- Log Analytics
- Application Insights

## Following components will need to be created as part of the solution
- An API
- Policy for the API
- App Service Plan within the ASEv3
- Storage Account
- Create Blob Container to store the log file
- Create File Storage for maintaining the Logic App hosts.json, workflow, paramter and connection files

## Overall Architectural solution will look like below:
![image](https://user-images.githubusercontent.com/43401999/154848583-6de229b5-143f-474d-a5bf-d8bef2f989e2.png)
