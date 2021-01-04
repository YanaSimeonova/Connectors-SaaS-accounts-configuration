 
# Configuring Aha OAuth account in webMethods.io Integration Workflow <br/>

## Summary:
   
This article describes about how to configure an OAuth App in Aha and configuring an account in webMethods.io workflow<br/> 

## Pre-requisites:
•	User must have a working Aha instance <br/>
•	Working webMethods.io tenant <br/> 

## Contents:

Section 1: Register OAuth application in Aha <br/> 
Section 2: Generate an access token <br/> 
Section 3: Configuring an OAuth Aha account in webMethods.io <br/> 


### Section 1. Register OAuth application in Aha <br/> 

 1. Login to your Aha instance <br/>

 2. Navigate to settings in the top right corner and select Developer in the left side <br/>

![Aha](images/1.png)<br/>

 3. Click on Register OAuth application and provide the Name of the App and Redirect URI and click create <br/>

![Aha](images/2.png)<br/>

 4. After creating the App - Redirect URI , Client ID , Client Secret , Authorize URL will be generated <br/>

![Aha](images/3.png)<br/>

### Section 2. Generate an access token <br/> 

 5.Copy Authorize URL and Paste the URL in Google and hit enter <br/>

![Aha](images/4.png)<br/>

 6.	Post Enter ,It will ask you to authorize the app <br/>
 
![Aha](images/5.png)<br/>

 7.	After authorizing the app , Access Token will be generated <br/>

![Aha](images/6.png)<br/>

Section 3: Setting up a Aha account in webMethods.io Integration tenant

 8.	Login to webMethods.io Integration tenant <br/>
 9.	Create new project or choose an existing project if required <br/>
 10.Click on workflows tab and add new workflow <br/>

![Aha](images/7.png)<br/>
 
 11. Name your workflow and then Drag and drop Aha from the connector pallet and double click on Aha connector to configure the account. <br/>

![Aha](images/8.png)<br/>

 12. Select action  and click on (+) to add account <br/>

![Aha](images/9.png)<br/>
 
 13.Enter all the required details and Click on “Add” to save the Account successfully. <br/>

![Aha](images/10.png)<br/>

 14.Connect the connector to stop and save the workflow and click on run to run the entire workflow <br/>

![Aha](images/11.png)<br/>
![Aha](images/12.png)<br/>




