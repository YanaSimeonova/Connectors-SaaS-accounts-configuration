
# Adobe Experience Platform (AEP) OAuth 2.0 Connection in webMethods.io

## Summary:

This article describes the step-by-step process of generating an Access token and configuring an account for the **Adobe Experience Platform** OAuth V2.0 Connection in webMethods.io<br/>

## Pre-requisites:
- User needs to have a working **Adobe Experience Platform** account to log into the Adobe cloud console
- Applicable on the API
- Access permission for **Adobe Experience Platform** APIs
- Working **webMethods.io** tenant
- Create Java Keystore Certificate(.jks) and export Public key certificate on your local machine or platform server machine

## Contents:

- How to generate an Access token for the **Adobe Experience Platform** APIs required for the OAuth 2.0 Authorization 
- Establishing a Connection in **webMethods.io Integration** tenant

## Configure API and generate an access token:

1.	Login to **console.adobe.io**

2.	Go to Projects tab, Create a new **Project**

3.	Click **Add API**
	
	![AEP](images/1.png)<br/>
	
4.	Select **Experience Platform API**
	
	![AEP](images/2.png)<br/>
	
5.	Configure API, Upload your public key certificate, and click **Next**
	
	![AEP](images/3.png)<br/>
	
6.	Click **Next** to create a new **Service Account(JWT)**
	
	![AEP](images/4.png)<br/>
	
7.	Select all the product profiles as applicable and Click **Save configured API**

	![AEP](images/5.png)<br/>

8.	Click **Service Account (JWT)** and open Credentials details<br/>
	Copy the following parameters required for account configuration in wM.io<br/>
	*CLIENT ID*<br/>
    *CLIENT SECRET*<br/>
    *TECHNICAL ACCOUNT ID*<br/>
    *ORGANIZATION ID*
 
	![AEP](images/6.png)<br/>
	
## Create a Connection for Adobe Experience Platform in webMethods.io

1.	Login to **webMethods.io Integration** tenant
	
2.	Create a **FlowService**

	![AEP](images/7.png)<br/>
	
3.	Enter **Adobe Experience Platform** and select the **Connector**

	![AEP](images/8.png)<br/>
	
4.	Select **Pre-defined Action** or **Add Custom Action** and Configure **Account**
	
	![AEP](images/9.png)<br/>
	
5.	**Add Keystore Certificate**<br/>
	Provide the location of the Keystore file(.jks) and enter the password used while generating **.jks**

	![AEP](images/10.png)<br/>
	
6.	Select the JWT Keystore alias added and also select the JWT key alias used while creating Keystore(default “1”)<br/>
	Generate Audience using ClientId,<br/>
	Syntax : https://ims-na1.adobelogin.com/c/ClientId<br/>
	Example : https://ims-na1.adobelogin.com/c/94ff378d74c84dc29ea9ee6a6bd43140<br/>
	Sandbox Name : prod

	![AEP](images/11.png)<br/>
	
7.	Enter the following properties and leave the other properties with default values or else enter the values as per  		  	  requirements while configuring the account,<br/>
		*Organization ID*<br/>
		*Technical Account ID*<br/>
		*JWT Keystore*<br/>
		*JWT Key Alias*<br/>
		*Audience*<br/>
		*Client ID*<br/>
		*Client Secret*<br/>
		*Sandbox Name*

8.	In case the user needs to use this account for the Streaming APIs, then user needs to add the SNI details as mentioned in 	  the below snapshot
	
	![AEP](images/12.png)<br/>

9.	The User needs to create a different account in case of the Streaming Ingestation APIs. Adobe enables the SNI Support for 	  the Streaming APIs

10.	Select the created AEP account and continue to create the required custom action
	
	![AEP](images/13.png)<br/>

11.	Once the action and the account are selected, execute the FlowService to verify the connection to **Adobe Experience 		Platform**
	
	![AEP](images/14.png)<br/>

	![AEP](images/15.png)<br/>

