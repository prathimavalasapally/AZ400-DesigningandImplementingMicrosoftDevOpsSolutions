## Instructions

### Getting Started with Lab

1. Once the environment is provisioned, a virtual machine (JumpVM) on the left and lab guide on the right will get loaded in your browser. Use this virtual machine throughout the workshop to perform the lab.

1. To get the lab environment details, you can select the **Lab Environment** tab, you can locate the **Lab Environment** tab on the upper right corner. Additionally, the credentials will also be emailed to your email address provided during registration.

### Task 1: Log in to Azure Portal

1. In the JumpVM, double click on the Azure portal shortcut on the desktop.
   
    > **Note:** In the welcome to Microsoft Edge page, select **Start without your data** and on the help for importing Google browsing data page select the **Continue without this data** button and procced to select **Confirm and start browsing** in the next page.

1. On **Sign in to Microsoft Azure** blade, you will see a login screen, in that enter the following email/username and then click on **Next**. 
  
1. Now enter the following password and click on **Sign in**.
   
1. In the pop-up for *Action Required*, select **Ask Later**.

1. If you see the pop-up **Stay Signed in?**, click Yes

1. If you see the pop-up **You have free Azure Advisor recommendations!**, close the window to continue the lab.

1. If a **Welcome to Microsoft Azure** popup window appears, click **Maybe Later** to skip the tour.

### Task 2: Create a DevOps organization

1. Navigate to [https://aex.dev.azure.com](https://aex.dev.azure.com).

2. On the **We need a few more details** page, select **Continue**.

3. In the drop-down box on the left, choose **Default Directory**, instead of “Microsoft Account”.

4. If prompted (*"We need a few more details"*), provide your name, e-mail address, and location and click **Continue**.

5. Back at [https://aex.dev.azure.com](https://aex.dev.azure.com) with **Default Directory** selected click the blue button **Create new organization**.

6. Accept the *Terms of Service* by clicking **Continue**.

7. If prompted (*"Almost done"*), leave the name for the Azure DevOps organization at default (it needs to be a globally unique name) and pick a hosting location close to you from the list.

8. Once the newly created organization opens in **Azure DevOps**, click **Organization settings** in the bottom left corner.

9. At the **Organization settings** screen click **Billing** (opening this screen takes a few seconds).

10. Click **Setup billing** and on the right-hand side of the screen select the **Azure Pass - Sponsorship** subscription and click **Save** to link the subscription with the organization.

11. Once the screen shows the linked Azure Subscription ID at the top, change the number of **Paid parallel jobs** for **MS Hosted CI/CD** from 0 to **1**. Then click the **SAVE** button at the bottom.

12. In **Organization Settings**, go to section **Security** and click **Policies**.

13. Toggle the switch to **On** for **Third-party application access via OAuth**
    > Note: The OAuth setting helps enable tools such as the DemoDevOpsGenerator to register extensions. Without this, several labs may fail due to a lack of the required extensions.

14. Toggle the switch to **On** for **Allow public projects**
    > Note: Extensions used in some labs might require a public project to allow using the free version.

15. **Wait at least 3 hours before using the CI/CD capabilities** so that the new settings are reflected in the backend. Otherwise, you will still see the message *"No hosted parallelism has been purchased or granted"*.
