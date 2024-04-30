Use 7-zip to unzip and combine the setup files.

TeamsLight Tool Setup Guide

TeamsLight relies on Microsoft Graph API, to use the tool, you need to follow the steps below to get Azure application ID and tenant ID with proper permissions on the application.
1.	Open browser, navigate to portal.auzre.com, click and open Microsoft Entra ID.

2.	In Microsoft Entra ID, go to Manage->App registrations, click on “New Registration” to register a new application.
 

3.	In Register an application form, enter name, then click on Register to register the application.
 
4.	When application is created, go to Overview page to get the Application ID and Tenant ID, save them in notebook.
 

5.	Go to Authentication, click on “Add a Platform” to configure platform, select “Mobile and desktop applications”.
 

6.	Use the Application ID saved in notebook to format the URI  ms-appx-web://microsoft.aad.brokerplugin/<appid>, for example ms-appx-web://microsoft.aad.brokerplugin/ b08d24d4-f93d-4dcb-8df4-0065029d82a5, put the URI in “Custom redirect URIs” and click Configure button to save, you will get platform setting.
 

7.	Go to API permissions, click on “Add a permission”, then select Microsoft Graph->Delegated permissions, add offline_access,openid,profile,Chat.Read,ChatMessage.Read,User.ReadBaisc.All.
 

After you add the permissions, you will get API permissions settings.
 

8.	After you register the application and finish the settings, open TeamsLight app, enter your  Application ID and Tenant ID saved in notebook, click Login button to login the tool.
 
