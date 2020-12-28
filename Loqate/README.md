

# Configuring Loqate account in webMethods.io Integration Workflow <br/>

## Summary:

This article describes configuring an account to **Loqate** in **webMethods.io Workflow**<br/>

## Pre-requisites:
•	User needs to have a **Loqate** account<br/> 
•	Working **webMethods.io Integration** tenant<br/> 

## Contents:

Section 1: Configure a **Loqate** account<br/> 
Section 2: Setting up a **Loqate** account in **webMethods.io Integration** tenant<br/> 

### Section 1. Configure a Google OAuth <br/>

1.  [Sign up](https://account.loqate.com/register/) to Loqate or [login](https://account.loqate.com/Login/?r=%2faccount%2f) if you already have an account. 

2.  Click on **Add service**,  In the Setup page , click on the API key<br/>

	![Loqate](images/1.png)<br/>

	![Loqate](images/2.png)<br/>

3.  Switch to configuration tab and configure your Loqate API key <br/>

    ![Loqate](images/3.png)<br/>

4. Note down **API key** <br/>

### Section 2: Setting up Loqate account in webMethods.io Integration Workflow<br/>

5. Login to **webMethods.io Integration** tenant and choose your project or click on **"+"** to create new project<br/>

6. Switch to **Connectors** tab<br/>

7. Search for **Loqate** connector in the available connectors list. <br/>

	![PubSub](images/4.png)<br/>

8. Mouse hover on the **Loqate** connector icon and then click on the **"+"** icon.<br/>

	![PubSub](images/5.png)<br/>

9. Fill in the **Account name**, **API key** obtained from Step 4 . Click on **Add**.<br/>

	![PubSub](images/6.png)<br/>

10. An account for Loqate connector has been added successfully, now you can use this account in your Workflows/Flowservices<br/>
