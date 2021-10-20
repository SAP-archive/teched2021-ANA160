# Exercise 0 - Setting up the environment

In this exercise you will learn how to prepare your environment for the actual part of this hands on session. Note that this session is based on trial accounts which are completely free of charge. We also recommend using (new) trial accounts in order to work in an isolated environment.

In particular we require having trials of **SAP HANA Cloud** and **SAP Web IDE** (on Cloud Foundry). Furthermore, a trial account for the **SAP Cloud Platform** is the starting point for the product trials, and is required as well.

## Exercise 0.1 - Creating a SAP Cloud Platform Trial Account

In order to create a SAP Cloud Platform Trial Account, you have to conduct the following steps. This trial account is required to start the SAP HANA Cloud and SAP Web IDE trial.

1. Create an account on [sap.com](https://www.sap.com): Navigate to that site, and click on the "person" pictogram in the right upper corner. You have to either create an account or login. In the course of the tutorial we will create a new account.
<br>![](/exercises/ex0/images/sap_com_account.png)

2. Please fill out the form with your details, and click on "Submit".

<br>![](/exercises/ex0/images/register1.png)

3. Please check your mailbox and verify your e-mail address, and click on the link.

<br>![](/exercises/ex0/images/register2.png)

4. Having verified your account, log into the SAP Cloud Platform Trial to start it on https://account.hanatrial.ondemand.com/ and after login you need to verify your account first. In order to do so, enter you mobile number, and a text message will be sent to your mobile.

<br>![](/exercises/ex0/images/verify1.png)

5. On the next screen enter this code. Your account is now verified.

6. As a next step you might have to choose the region thats close to you, choose one and click on "create account"

<br>![](/exercises/ex0/images/choose_region.png)

7. The actual account setup will take a bit, and your screen will look like this, click on continue once those steps are done:

<br>![](/exercises/ex0/images/account_creation.png)

8. Now your account is verified, your screen should look like this:

<br>![](/exercises/ex0/images/start_sap_cp_trial.png)

Even more detailed instructions can be found here: https://developers.sap.com/tutorials/hcp-create-trial-account.html.

## Exercise 0.2 - Creating an SAP HANA Cloud Trial Instance

After having created your SAP Cloud Platform Trial Account, you should proceed to creating an SAP HANA Cloud Trial instance. Please make sure you remember the password you will set for the DBADMIN user, since we will need this later. In order to do so, please follow the following steps:

1. After you logged into your SAP Cloud Platform Trial account, select your "trial" subaccount.

<br>![](/exercises/ex0/images/enter_trial1.png)

2. Select the "dev" space.

<br>![](/exercises/ex0/images/enter_trial2.png)

3. Click on the menu entry "SAP HANA Cloud"

<br>![](/exercises/ex0/images/enter_trial3.png)

4. Now we create a new instance by clicking on "Create Instance"

<br>![](/exercises/ex0/images/create_instance1.png)

5. Add an instance name and set the DBADMIN Password (please remember this for later). Click on "Step 2" to continue.

<br>![](/exercises/ex0/images/create_instance2.png)

6. We cannot configure the sizing (since this is a trial), so click on "Step 3"

<br>![](/exercises/ex0/images/create_instance3.png)

7. We do not need a data lake for this demo either, so click on "Step 4"

<br>![](/exercises/ex0/images/create_instance4.png)

8. For this tutorial we **DO** require that you allow all external IP addresses to access your SAP HANA Cloud instance. In particular, in step 4, please choose the option as shown in the screenshot below.  This is necessary to allow the Web IDE to access your instance during deployment. For a productive setup, you might consider limiting the IP address ranges, but in order to make it simple for this tutorial, we allow all. This setting can also be changed after instance creation, i.e., limits can also be applied afterwards. Once this is set, click on "Create Instance" to start the creation process.

<br>![](/exercises/ex0/images/hana_cloud_set_ip_to_all.png)

8. The system indicates that the instance is being created, and at the end it should be running.

<br>![](/exercises/ex0/images/hana_cloud_running.png)

Addional information can be found here:

- https://saphanajourney.com/hana-cloud/learning-article/starting-a-sap-hana-cloud-trial-when-you-have-an-existing-sap-cloud-platform-trial/
- https://saphanajourney.com/hana-cloud/learning-article/how-to-create-your-trial-sap-hana-cloud-instance/ 

After having created and started your SAP HANA Cloud Trial instance, continue with the User Creation.

## Exercise 0.3 - Creating the required users

Throughout this whole exercise we require three SAP HANA users that represent the personas as outlined. In order to have them ready once required, we create them now. We will create the user *HR_SUPERVISOR*, *HR_CALL_CENTER_AGENT* and *DATA_SCIENTIST*

1. Navigate to your SAP HANA Cloud trial tile, and open the SAP HANA Cockpit
<br>![](/exercises/ex0/images/open_hana_cockpit.png)
2. As the new browser windows open, you might be asked for database credentials. Please enter the credentials of the *DBADMIN* user including the password set during the creation of the trial instance.
3. Navigate to "Security and User Management" in the database overview.
<br>![](/exercises/ex0/images/security_user_management.png)
4. Open "User Management"
<br>![](/exercises/ex0/images/user_management.png)
5. In order to create a new user, click the "+" in the Users section and choose "Create User":
<br>![](/exercises/ex0/images/add_user1.png)
6. Fill out the form to create a new user, in particular, set the username to *HR_SUPERVISOR*, set a password and (**important**) do not forget to check "No" for forcing the user to set a new password after the first logon. Please remember the password, we will need that later.
<br>![](/exercises/ex0/images/add_user2.png)
7. Once done with the form, click the "Save" button to create the user.
<br>![](/exercises/ex0/images/add_user3.png)
8. Please repeat these steps to create the *HR_CALL_CENTER_AGENT* and the *DATA_SCIENTIST* users.

As a last step, we continue with the SAP Web IDE trial.

## Exercise 0.4 - Creating an SAP Web IDE Trial Instance

Within your SAP Cloud Platform Trial, you have to subscribe to the SAP Web IDE as well for this hands-on session. 

1. Navigate to your "trial" subaccount by clicking on the subaccount in the topmost bar

<br>![](/exercises/ex0/images/webidesub1.png)

2. Click on Subscriptions in the menu, and choose the SAP Web IDE

<br>![](/exercises/ex0/images/webidesub2.png)

3. A new window opens, click on the blue "Subscribe" Button to subscribe to the Web IDE, the status will change to a green "Subscribed".

<br>![](/exercises/ex0/images/subscribe_webide.png)


4. Click on "Go to application" and bookmark the SAP Web IDE URL, we will need that later.

<br>![](/exercises/ex0/images/webidesub3.png)

**Important Note:** While opening the SAP Web IDE there *might* be a message stating that support for the WebIDE will end on November 13th. Please ignore this message.

<br>![](/exercises/ex0/images/webide_discontinued.png)

More Information can be found here: https://developers.sap.com/tutorials/webide-multi-cloud.

## Summary

We are now fully set up and can start with the actual hands on exercise. In the very next step, we will upload the demo project, to have an environment with data.

Continue to - [Exercise 1 - Setting up the Web IDE Project](../ex1/README.md)