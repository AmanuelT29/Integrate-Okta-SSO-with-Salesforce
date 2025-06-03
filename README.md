<p align="center">
<img src="https://cdn.worldvectorlogo.com/logos/okta-logo.svg" alt="Okta Logo" width="170"/>   <img src="https://cdn.worldvectorlogo.com/logos/salesforce-2.svg" alt="Salesforce Logo" width="150"/>


#  Okta SSO Integration with Salesforce


## Platform and Tools Used

- Okta
- Salesforce
- Web Browser


## Objective

In this project, I aim to demonstrate how to integrate Okta Single Sign-On (SSO) with the Salesforce application. The process begins by creating four new users in both Okta and Salesforce. Next, I create a "Marketing" group in Okta and assign the new users to this group to implement Role-Based Access Control (RBAC). I then configure the Salesforce application in Okta and set up SSO integration. Finally, I assign the Marketing group to the Salesforce application, granting users access and ensuring a successful SSO implementation.
 
-----

### Create Users and Group on Okta

1. Started by adding new users **Oly** and **Monisha**, and followed the same process for the remaining users:

<img src="https://github.com/user-attachments/assets/c1fef801-1c50-4795-8b9d-f09603455cca" alt="Screenshot 1" width="300"/>
<img src="https://github.com/user-attachments/assets/5d2bfc2c-9cce-4281-8154-5f8597e50064" alt="Screenshot 2" width="300"/>
</p>

  
2. Navigated to **People** to verify that all four users were successfully added:

   <img src="https://github.com/user-attachments/assets/01da420e-7128-449b-b836-19f6e61b1a08" alt="Screenshot" width="500"/>

   
3. Navigated to **Groups** to add **Marketing** Group:
   
   
<img src="https://github.com/user-attachments/assets/f09a07d1-8718-4fdd-91db-27b1d9e1c3d7" alt="Screenshot" width="500"/>


4. Navigated to **Groups** to verify **Marketing** is successfully added:

<img src="https://github.com/user-attachments/assets/675afafb-6479-4096-a835-73921e5fb051" alt="Screenshot" width="500"/>
</p>

### Assign Users to Groups

1. Navigated to the **Marketing** group and assigned users by clicking the plus sign:
   
<img src="https://github.com/user-attachments/assets/e8d83c5b-1d8c-4e04-958e-f736d7e7d8ae" alt="Screenshot" width="500"/>

2. Confirmed all the users are successfully added to **Marketing** group:

<img src="https://github.com/user-attachments/assets/92ccf1fa-70d1-4241-a0a6-7b5ab0853001" alt="Screenshot" width="500"/>


### Add Users on Salesforce

1. Navigated to **Users** on Salesforce and added the users I created on Okta. Followed the same process for the remaining users:

<img src="https://github.com/user-attachments/assets/7ea7f90a-d1d2-42e8-9f64-41f0105249e0" alt="Screenshot 1" width="500"/>
<img src="https://github.com/user-attachments/assets/6b4cc41b-70c6-4e6d-b768-842b028d99f7" alt="Screenshot 2" width="500"/>





### Integrate Okta with Salesforce Application
1. To find Salesforce on Okta:
   
   - Go to Applications > Browse App Integration Catalog > Search for Salesforce > Click on Salesforce:

<img src="https://github.com/user-attachments/assets/37433212-aaab-4f67-807b-df88fbc38508" alt="Screenshot" width="500"/>

2. Click Add Integration:

<img src="https://github.com/user-attachments/assets/ed7dca0e-0dba-4ea1-a409-d247cd2c612f" alt="Screenshot" width="600"/>

3. Since this is a testing project and not a real deployment, switch to a Sandbox under the instance type option:

<img src="https://github.com/user-attachments/assets/d86078ab-9832-4a86-bb24-eb29fd37457e" alt="Screenshot" width="400"/>


### Configure SAML 2.0 for Salesforce

1. In Okta’s **Salesforce.com Sign-On Options** settings, switch to **SAML 2.0**, as it is required for SSO implementation:

<img src="https://github.com/user-attachments/assets/fba32da6-10f0-42e5-863d-73b77be486ca" alt="Screenshot" width="400"/>

2. To configure SSO on Salesforce website: **Identity**>**Single Sign-On Settings**:
   
   - Click edit and check mark **SAML Enabled**:
 <img src="https://github.com/user-attachments/assets/b860e2d1-1411-4d2f-8ccb-a58e34133ecf" alt="Screenshot" width="400"/>

3. Used Okta's **How to Configure SAML 2.0 for Salesforce** guidlines to configure **SAML Single Sign-On Settings**:

 <img src="https://github.com/user-attachments/assets/a19c2b03-7500-4694-bc94-bd47c310cf1a" alt="Screenshot" width="500"/>

4. Copied and pasted the **Login URL** provided by Salesforce into Okta’s Salesforce **Login URL** field:

  <img src="https://github.com/user-attachments/assets/6718f2ec-69f2-45fd-98dd-5adbe909dcdc" alt="Screenshot" width="400"/>

5. Confirmed Salesforce is successfully integrated on Okta:

 <img src="https://github.com/user-attachments/assets/fbab4717-2d77-4772-8c41-b3ee08a4df3c" alt="Screenshot" width="400"/>


### Assign Group to Salesforce Application

1. To assign **Marketing** group to Salesforce application:

   - Go to Application>SalesForce>Assign to Groups>Marketing>Assign:
   
<img src="https://github.com/user-attachments/assets/a405d87e-00a8-42de-93c7-aa028ee9a472" alt="Screenshot 1" width="450"/>
<img src="https://github.com/user-attachments/assets/fb66873d-e55e-4816-824d-1ad92f42ac3d" alt="Screenshot 2" width="450"/>
</p>


2. Confirmed **Marketing** group and all user belonging in the group are assigned to Salesforce application:

<img src="https://github.com/user-attachments/assets/b936add7-6416-4bc3-9ef9-33947f5d8acb" alt="Screenshot 1" width="450"/>
<img src="https://github.com/user-attachments/assets/8ed50b6e-fd12-434f-a835-48879de3513d" alt="Screenshot 2" width="450"/>


### Verify Salesforce is Successfully Integrated on the User's Okta Dashboard

- As shown in the screenshots, all four users in the **Marketing** group have the Salesforce application in their Okta account:

<img src="https://github.com/user-attachments/assets/cdc1605a-aeae-4661-9280-e5ddf2c5e740" alt="Screenshot 1" width="45%" />
<img src="https://github.com/user-attachments/assets/68515c8f-0bf6-4acc-884f-187eb188a3f6" alt="Screenshot 2" width="45%" />

<img src="https://github.com/user-attachments/assets/f7eb95ba-0011-4b1d-a287-b90154172f77" alt="Screenshot 3" width="45%" />
<img src="https://github.com/user-attachments/assets/0ca71f26-d79e-417e-bfda-28960403888a" alt="Screenshot 4" width="45%" />


### Verify successful user SSO access to Salesforce from Okta

- As shown in the screenshots, all four users in the **Marketing** group were able to access Salesforce via SSO from Okta:

<img src="https://github.com/user-attachments/assets/1c3575c2-c261-43f0-8e0c-07c2704d8de0" alt="Screenshot 5" width="400" />
<img src="https://github.com/user-attachments/assets/5d53944f-5d93-4e69-88d8-ca61f2da7e5d" alt="Screenshot 6" width="400" />


<img src="https://github.com/user-attachments/assets/97f47bbe-09a1-40ca-9f44-a9dda4bd5eb2" alt="Screenshot 7" width="400" />
<img src="https://github.com/user-attachments/assets/03f3a632-3520-4447-9113-f6d901c1f9dd" alt="Screenshot 8" width="400" />


---

## Conclusion

This project successfully demonstrates the integration of Okta Single Sign-On (SSO) with Salesforce, streamlining user access management through centralized authentication. By creating **users** and organizing them into a **Marketing** group within Okta, Role-Based Access Control was effectively implemented. The configuration of SAML 2.0 ensured secure and seamless SSO between Okta and Salesforce. Verification steps confirmed that all assigned users could access Salesforce directly from their Okta dashboards without issues. Overall, this integration enhances security, simplifies user management, and improves the user experience for accessing Salesforce





