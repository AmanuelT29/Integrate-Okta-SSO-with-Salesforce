<p align="center">
<img src="https://cdn.worldvectorlogo.com/logos/okta-logo.svg" alt="Okta Logo" width="170"/>   <img src="https://cdn.worldvectorlogo.com/logos/salesforce-2.svg" alt="Salesforce Logo" width="150"/>


#  Okta SSO Integration with Salesforce


## Platform and Tools Used


## Objective

In this project, I demonstrate how to integrate Okta Single Sign-On (SSO) with the Salesforce application. The process begins by creating four new users in both Okta and Salesforce. Next, I create a "Marketing" group in Okta and assign the new users to this group to implement Role-Based Access Control (RBAC). I then configure the Salesforce application in Okta and set up SSO integration. Finally, I assign the Marketing group to the Salesforce application, granting users access and ensuring a successful SSO implementation.
 
-----

### Create Users and Group on Okta

1. Started by adding new users **Monisha** and **Oly**, and followed the same process for the remaining users.

  <img src="https://github.com/user-attachments/assets/012554c1-b8c0-45ad-b465-0808b232d6e7" alt="Screenshot 1" width="350"/>
  <img src="https://github.com/user-attachments/assets/1228a06f-9ca4-4180-a1dd-b33db668e6c8" alt="Screenshot 2" width="350"/>
</p>

2. Navigated to **People** to verify that all users were successfully added.

   <img src="https://github.com/user-attachments/assets/01da420e-7128-449b-b836-19f6e61b1a08" alt="Screenshot" width="450"/>

   

3. Navigated to **Groups** to add **Marketing** Group.
   
   
<img src="https://github.com/user-attachments/assets/f09a07d1-8718-4fdd-91db-27b1d9e1c3d7" alt="Screenshot" width="400"/>


4. Navigated to **Groups** to verify **Marketing** is successfully added.

![Screenshot 2025-06-02 204948](https://github.com/user-attachments/assets/675afafb-6479-4096-a835-73921e5fb051)

### Assign Users to Groups

1. Navigated to the **Marketing** group and assigned users by clicking the plus sign.
   
![Screenshot 2025-06-02 205925](https://github.com/user-attachments/assets/e8d83c5b-1d8c-4e04-958e-f736d7e7d8ae)

2. Confirmed all the users are successfully added to **Marketing** group

![Screenshot 2025-06-02 211519](https://github.com/user-attachments/assets/92ccf1fa-70d1-4241-a0a6-7b5ab0853001)


### Add Users on Salesforce

1. Navigated to **Users** on Salesforce and added the users I created on Okta. Followed the same process for the remaining users.

<img src="https://github.com/user-attachments/assets/7ea7f90a-d1d2-42e8-9f64-41f0105249e0" alt="Screenshot 1" width="500"/>
  <img src="https://github.com/user-attachments/assets/6b4cc41b-70c6-4e6d-b768-842b028d99f7" alt="Screenshot 2" width="500"/>
</p>




### Intergrate Okta with Salesforce Application

### Configure Salesforce

### Assign to Salesforce Application

### Check if Salesforce is Successfully Integrated on the User's Okta Dashboard

### Confirm Successful User Access to Salesforce from Okta
