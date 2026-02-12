# Bypass SSO for Salesforce REST API Connectivity through Boomi

## Problem Statement:
When we configure the Environment Extension in Boomi for a Salesforce REST Connector, such as Salesforce Platform Event Connector or HTTP Client Connector (using OAuth2.0 as the Authentication Type and Authorization Code as the Grant Type), we have to generate the Access Token using the Password for the first time, through the Salesforce Login UI. We will have to do the same as a one-time activity when Salesforce password is refreshed. When only SSO login is enabled for the Boomi integration user, then the login won't be possible. 

## Solution:
**Step-1:** Login to Salesforce, preferably as an Admin user.

**Step-2:** Go to Home --> Enter "My Domain" in the search bar on the left side of the page.

<img width="336" height="336" alt="image" src="https://github.com/user-attachments/assets/f2edb6a0-dfda-412c-b1f3-d8f652956746" />

**Step-3:** Select the "Login Form" checkbox and click Save.

<img width="1010" height="824" alt="image" src="https://github.com/user-attachments/assets/f7793785-7ea8-4e37-9cf6-e3d45078f395" />

**Step-4:** Go to Boomi Environment Extension --> Select the relevant Connection --> Click the Generate/Regenerate button. This will open a new tab where the Salesforce Login UI will show up. Enter username and password, and once the Access Token is successfully generated, click the Save button in the Boomi Environment Extension.

<img width="369" height="136" alt="image" src="https://github.com/user-attachments/assets/551ee2d8-30d7-43cc-be18-673bbb45ecad" />
