# 03 - Create blob storage

In this walkthrough, we will create a storage account, then work with blob storage files.

# Task 1: Create a storage account

In this task, we will create a new storage account. 

1. Click on the Azure Portal icon on the VM desktop and login with the Azure credentials from the Lab Environment output page.

2. From the **All services** blade, search for and select **Storage accounts**, and then click **+ Create**. 

3. On the **Basics** tab of the **Create storage account** blade, fill in the following information (replace **xxxx** in the name of the storage account with the deployment ID). Leave the defaults for everything else.

    | Setting | Value | 
    | --- | --- |
    | Subscription | **Choose your subscription** |
    | Resource group | **Azure-Researcher-[DeploymentID]** (use existing) |
    | Storage account name | **storageaccountxxxx** |
    | Location | **(US) East US**  |
    | Performance | **Standard** |
    | Redundancy | **Locally redundant storage (LRS)** |


5. Click **Review** to review your storage account settings and allow Azure to validate the configuration. 

6. Once validated, click **Create**. Wait for the notification that the account was successfully created. 

7. From the Home page, search for and select **Storage accounts** and ensure your new storage account is listed.

    ![Screenshot of the newly created storage account in the Azure portal .](../images/0401.png)

# Task 2: Work with blob storage

In this task, we will create a Blob container and upload a blob file. 

1. Click the name of the new storage account, scroll to the **Data storage** section, and then click **Containers**.

2. Click **+ Container** and complete the information. Use the Information icons to learn more. When done click **Create**.

   | Setting | Value |
   | ---- | ---- |
   | Name | **container1**|
   | Public access level| **Private (no anonymous access)** |
    
    ![Screenshot of the newly created blob container in the storage account in the Azure portal.](../images/0402.png)

4. Click the **container1** container, and then click **Upload**.

5. Browse to a file on your local computer. 

    **Note**: You can create an empty `.txt` file or use any existing file. Consider chooosing a file of a small size to minimize the upload time.

6. Click the **Advanced** arrow, leave the default values but review the available options, and then click **Upload**.

    **Note**: You can upload as many blobs as you like in this way. New blobs will be listed within the container.

7. Once the file is uploaded, right-click on the file and notice the options including View/edit, Download, Properties, and Delete. 

8. As you have time, from the storage account blade, review the options for Files, Tables, and Queues.

# Task 3: Monitor the storage account

1. If needed, return to the storage account blade and click **Diagnose and solve problems**. 

2. Explore some of the most common storage problems. Notice there are multiple troubleshooter.

3. On the storage account blade, scroll down to the **Monitoring** section and click **Insights**. Notice there is information on Failures, Performance, Availability, and Capacity. Your information will be different.

    ![Screenshot of the storage account Insights page.](../images/0403.PNG)

Congratulations! You have created a storage account, then worked with storage blobs.
