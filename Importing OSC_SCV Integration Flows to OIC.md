# **Importing OSC_SCV Integration Flows to OIC**

### Prerequsite
1. Access to Oracle Integration Cloud. If you don't have cloud account, please sign up your free trial account here.
2. Log In Credentials of Oracle Sales Cloud
3. Log In Credentials of Oracle Services Cloud


### STEP 1: Importing the OIC integration flows
1. Open the link on Demo Central https://demo.oracle.com/apex/f?p=DEMOSTORE:15:5169485753648:::15:P15_DOC_ID:28748, and download the OSC-SVC.par to your local computer. You can also download the Click Through Demo and Configuration docx for more information.

2. Sign in to the Oracle Integration Cloud Service instance.
3. On the Welcome page, click the Intergation icon.
4. On Integration page, click the Packages icon
5. On the top right coner, click the Import Package button.
6. On Import Package File dialog box, browse the OSC_SVC.par and select it, then click Import Package.
> This creates all the integration flows contained within the package as well as the connections to Oracle Sales Cloud and Oracle Service Cloud. Next step is to configure the Oracle Service Cloud and Oracle Sales Cloud connections.

### Step 2: Configuring the Connection to the Oracle Sales Cloud Instance

1. On the Oracle Integration Cloud Service homepage, click the Connections icon.

2. On the Connections page, search for Oracle Sales Cloud and click on it for more details.

3. Click the Configure Connectivity button and in the Connection Properties window, enter the values of Sales Cloud

4. when you finish, click OK.

5. Click the Security Configuration button, and in the Credentials window, enter the LogIn Credentials:

6. Click OK.

7. Click the Test icon on the Oracle Integration Cloud Service Connection Configuration page.

8. When the status meter shows 100% Complete, click Save.

9. Click the Exit button.

## Step 3: Configuring the Connection to the Oracle Service Cloud Instance

After configuring the connection to the Oracle Sales Cloud instance, you then configure the connection to the Oracle Service Cloud instance.

1. On the Connections page, search for Oracle Service Cloud and click it for more details.

2. Click the Configure Connectivity button and in the Connection Properties window, enter the values of Service Cloud

3. when you finish, click OK.

4. Click the Security Configuration button, and in the Credentials window, enter the LogIn Credentials:

5. Click OK.

6. Click the Test icon on the Oracle Integration Cloud Service Connection Configuration page.

7. When the status meter shows 100% Complete, click Save.

8. Click the Exit button.

### Step 4: Activating the Integration Package
> To activate the integration flows you must have successfully imported the OSC_SVC integration package and configured Oracle Sales Cloud and Oracle Service Cloud connections.

1. Click Integrations icon on the left menu.

2. Locate OSC_SVC_CONTACT_CREATE, and click the Active button.

3. Check the Enable detail tracing check box and click the Active button on the confirmation dialog window.

4. Ensure the flow was activated successfully.

5. Repeat the active steps for the following integration flows:
OSC_SVC_ACCOUNT_CREATED
OSC_SVC_ACCOUNT_UPDATED
OSC_SVC_CONTACT_UPDATED
> After activation, verify that the integration synchronization is functional. Do this, for example, by creating or updating an account or contact record in the Oracle Sales Cloud. This action should automatically synchronize the record to Oracle Service Cloud. Additionally, create or update an organization or contact record in the Oracle Service Cloud. This action automatically synchronizes the record to Oracle Sales Cloud.

6. Repeat the activate steps for the following integration flows in the Oracle Service Cloud-to-Oracle Sales Cloud direction.
SVC_OSC_ORGANIZATION_CREATED
SVC_OSC_ORGANIZATION_UPDATED
SVC_OSC_CONTACT_CREATED
SVC_OSC_CONTACT_UPDATED
> Verify that the flows have been activated by signing in to Oracle Service Cloud and creating and updating organizations and contacts.