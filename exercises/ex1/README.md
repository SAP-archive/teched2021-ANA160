# Exercise 1 - Self-Service Data Preparation

 ![image001](../Images/image001.jpg)

<p align="center">
<B>SAP Data Intelligence Cloud</b>
</p>

<p align="center">
<b>Data Intelligence Self-Service Data Preparation</b>
</p>

- - - -


## Exercise 1.1 - Introduction
Welcome to our technical hands on section. This section which is based on SAP Data Intelligence Cloud focusses on the Self-Service Data Preparation capabilities provided by SAP Data Intelligence.

## Business Scenario
In this section, we are going to solve a real business challenge by transforming and publishing a dataset using the Self-Service Data Preparation feature for SAP Data Intelligence. 

Business users and data scientists can access, transform, and enrich datasets using a spreadsheet-like user interface in Metadata Explorer.

Use data preparation to find data quality issues, correct and standardize data, and then output the data for analysis. This process improves efficiency and gains better business insights.

Use the Data Preparation user interface in Metadata Explorer to view a set of data and create a recipe of actions to shape the data. The system puts these actions into a pipeline, also known as a graph. After processing the preparation, the transformed data is output into a target data set that other downstream applications can use. The Data Preparation user interface creates the graph for you so you do not have to find and configure the operators in the Modeler to create a graph.


At the conclusion of this exercise, you will be able to:
	
* Profile data from different sources
* Collect additional metadata
* Perform data transformation
* Publish transformed data
* Share data with downstream systems (Data Lake)

SAP Data Intelligence Metadata Explorer helps in managing data across systems. The Metadata Explorer helps in making informed decisions about different organizational datasets by profiling and publishing metadata. Users can preview data in the datasets and profile data to view information about the contents of different datasets.
We will use metadata management to profile our customer and business partner data sets from different sources and determine the quality of each dataset. We will also collect additional metadata like the minimum, maximum, averages, completeness, validity of data values. This information will help us determine which datasets need cleansing, masking, or additional operations when we model the data in Modeler application.

**Let's get started!**

:information_source: **``Your Instructor will provide you the SAP Data Intelligence Cloud URL and a Username/Password to login. The username is in the format of AC####U## i.e AC3357U01.``**

   - Log on using the following information:
   

![image003](../Images/image003.1.jpg)

<br>

You will see the ``SAP Guided Tours`` popup appear once you have successfully logged in. Please continue by selecting ``Close`` as indicated below. 

![image004](../Images/image001.1.jpg) 

<br>


## Exercise 1.2 - Metadata Explorer

In the SAP Data Intelligence Launchpad, click on Metadata Explorer tile. This will open the Metadata Explorer.


![image015](../Images/image015.jpg)

The Metadata Explorer Home page contains options help you search for data on a connection, create data preparations, profile or publish a dataset, create rules or a business glossary, monitor tasks, or modify your user preferences,

![image016](../Images/image016.jpg)

<br>

## Exercise 1.3 - Browse Connections

Open Browse Connections by choosing Catalog -> Browse Connections. The connections that we created in the Connection Management application are listed, select the ``list View`` option for more connection details.

![image017](../Images/image017.jpg)

<br>

You may filter the connections to view your connection easily. Type ``DI_TA_CONN`` in the ``"Filter Connection names"`` and filter the result set.

![image018](../Images/image018.jpg)

Open the SAP Hana Cloud connection by clicking on the ``DI_TA_CONN`` link. After the ``DI_TA_CONN`` connection is selected, filter and select **``ANA160``** schema where our data table is stored **``EMOBILITY_BOOT_NOTIFICATIONS``**. 

![image019](../Images/image019.jpg)


<br>


## Exercise 1.4 - Profile Data

To gain more information on a particular dataset ``Data Intelligence`` has the capability of running profiling tasks on the desired dataset to help us learn more about your data and where it could be lacking information.


Take note that in our system the **``EMOBILITY_BOOT_NOTIFICATIONS``** table is already profiled. 

<br>

:information_source:    ***``You will be profiling your own dataset later on in this hands-on.``***





<!-- ***``You will be profiling your own dataset later on in this hands-on.``*** -->

<br>

![image020](../Images/image020.jpg)

<br>

Let's go ahead and explore a ``profiled`` dataset by using the **``Fact Sheet``**.


<br>

## Exercise 1.5 - View Fact Sheet

For any profiled dataset you can view the Fact Sheet. Select ``view Fact Sheet`` icon.

![image022](../Images/image022.jpg)

<br>

The profiling result shows several metadata facts about the dataset. Notice the total rows in the table, show statistics on each column in the table. The statistics include ``minimum``, ``maximum``, ``average`` ``length``, ``% NULLs`` and ``blanks`` as well as ``distinct`` values and uniqueness by column.

![image023](../Images/image023.jpg)

<br>

Scroll Down:

![image024](../Images/image024.jpg)

<br>

Click on Columns:

![image025](../Images/image025.jpg)

<br>

You can click on a column to show statistics for the selected column type.

![image026](../Images/image026.jpg)

<br>

Scroll down on the next screen: 

![image027](../Images/image027.jpg)

<br>

You may preview the data by clicking the data preview tab

![image028](../Images/image028.jpg)

<br>


## Exercise 1.6 - Prepare Dataset

Next, we will **prepare** the dataset to standardize the content. 

Click on **Prepare data** to start data preparation

![image029](../Images/image029.jpg)

<br>

***Notice** that the ``TS`` column is native type of ``NVARCHAR`` instead of ``TIMESTAMP``. We must convert these values to ``TIMESTAMP``. 

First we need remove and replace the placeholder letter ``T`` with a single ``SPACE`` and placeholder ``Z`` at the end of the string with nothing.

<br>


Select ``Actions`` and ``Modify "TS"``.

![image030](../Images/image030.1.jpg)

<br>


Select the ``Replace`` action.



<!-- ![image030](../Images/image030.jpg) -->

![image030](../Images/image030.2.jpg)

<br>

<blockquote>
<p><strong>❗️ Important</strong>: Remember  Replace "T"  with a single  SPACE and click Apply</p>
</blockquote>

<!-- :bangbang: **Important!** ``Remember  Replace "T"  with a single  SPACE and click Apply`` -->

<!-- **``Remember  Replace "T"  with a single  SPACE and click Apply``** -->


![image030](../Images/image030.3.jpg)

<br>

***Note** that the data was updated and the the placeholder character ``T`` was replaced by a single space!

![image030](../Images/image030.4.jpg)

<br>

Let's remove placeholder character ``Z`` by using the ``Replace`` action as we have done in the previous step for letter ``T``.

![image030](../Images/image030.5.jpg)

<br>

<blockquote>
<p><strong>❗️ Important</strong>: Leave Replace by: blank and Apply the changes.</p>
</blockquote>

<br>

<!-- :bangbang: **Important!** ``Leave Replace by: blank and Apply the changes.`` -->



![image030](../Images/image030.6.jpg)

<br>

Verify that both special placeholder characters are replaced and removed.

![image030](../Images/image030.7.jpg)

<br>

Select the ``TS`` column and from the Actions available on the right, select action ``Convert To Date/Time``. Select ``yyyy-MM-dd HH:mm:ss.SSS`` format from the choices and click apply.

![image031](../Images/image031.jpg)

![image032](../Images/image032.jpg)

![image032](../Images/image032.1.jpg)

<br>

***Notice** that the values in the ``TS`` column have been converted to ``TIMESTAMP``.

<!-- There are a host of preparation options available. You may need to use other options to implement additional preparations. In this exercise, we are showing only 1 transformation. -->

We are now ready to run the preparation by selecting ``Run Preparation`` option as stipulated below. Click on ``Actions`` and select ``Run Preparation``.

![image033](../Images/image033.7.jpg)

Let's run the preparation and save the transformed dataset to the data lake ``DI_DATA_LAKE`` by selecting the target connection as the ``Connection Name``.

**``DI_DATA_LAKE`` is a shared filesystem provided by SAP Data Intelligence Cloud.**


<!-- ![image033](../Images/image033.jpg) -->

![image033](../Images/image033.1.jpg)

![image033](../Images/image033.2.jpg)

<br>

<blockquote>
<p><strong>❗️ Important</strong>: Click on Container to browse and select the teched2021-ANA160 folder where the data file will stored.</p>
</blockquote>

<!-- :bangbang:  **Important!** ``Click on Container to browse and select the teched2021-ANA160 folder where the data file will stored.`` -->

<br>

![image033](../Images/image033.3.jpg)

Click on the ``shared`` folder tile.

![image033](../Images/image033.4.jpg)

<br>

select the ``teched2021-ANA160`` subfolder.

![image033](../Images/image033.5.jpg)

<br>

You will now see the contents of the subfolder ``teched2021-ANA160`` 

***Note** There might be existing files already present **PLEASE** ignore this and select ``Apply``.


![image033](../Images/image033.8.jpg)





<br>

<blockquote>
<p><strong>❗️ Important</strong>:  Specify the Dataset Name, replace AC3538U01 with the username that was supplied to you. We will save the data in CSV format.</p>
</blockquote>

<!-- :bangbang:  **Important!** `` Specify the Dataset Name, replace AC3538U01 with the username that was supplied to you. We will save the data in CSV format.`` -->


![image033](../Images/image033.6.jpg)


<br>

## Exercise 1.7 - Publish Dataset

So far, we have profiled and prepared our dataset and changed the ``TS`` column to the required data type of ``TIMESTAMP``. Now, **navigate back** to the Browse Connection screen so that we can publish the data.

<br>

![image034](../Images/image034.jpg)

<br>

Select the ``DI_DATA_LAKE`` connection.

![image035](../Images/image035.jpg)

<br>

Select the ``shared`` subfolder.

![image035](../Images/image035.1.jpg)

<br>

Select the ``teched2021-ANA160`` subfolder.


![image035](../Images/image035.2.jpg)

<br>

We will now publish the dataset that we transformed and saved to the ``DI_DATA_LAKE`` target, so it becomes accessible to other users.

Select New Publication from transformed dataset in the Data Lake.

This will open the Publication section on the right.

![image036](../Images/image036.jpg)

Fill in the relevant fields and click on the Publish button.
**Use below name:** 
* Emobility Notifications EMOB_`<workshop ID>U<group number>`
* e.g. **EMOB_AC3538U01**

![image037](../Images/image037.jpg)

<br>


***Note It takes between 2 - 5 minutes to Publish**

<br>

Refresh by selecting the ``Refresh`` button as indicated until your file appears.

![image039](../Images/image039.4.jpg)

<!-- ![image037](../Images/image037.1.jpg) -->

<br>

After publishing the dataset, refresh the "Browse Connections" section to see the dataset has been published in the ``DI_DATA_LAKE`` ``/shared/teched2021-ANA160`` target location.

![image038](../Images/image038.jpg)

<!-- <br>

Refresh by selecting the ``Refresh`` button as indicated.

![image039](../Images/image039.4.jpg) -->

<br>


The data transformation is now ready for integration. We will also profile the dataset.


![image039](../Images/image039.jpg)

![image039](../Images/image039.1.jpg)

<br>

***Note It takes between 2 - 5 minutes to Profile**

<br>

Use the Refresh Button to update the Page



![image039](../Images/image039.2.jpg)

![image039](../Images/image039.3.jpg)

<br>

## Exercise 1.8 - Data Lineage

We finished profiling and publishing our datasets. Next, we will now observe our changes from ``source`` to ``target`` by using the ``Data Lineage`` feature.

Start by selecting the ``Lineage`` option as indicated below, keep in mind this is on our newly transformed data set stored in the ``DI_DATA_LAKE`` shared filesystem. 

![image039](../Images/image094.jpg)

<br>

Let's look at the ``SAP Hana Cloud`` based ``source`` staging table ``EMOBILITY_BOOT_NOTIFICATIONS`` by clicking on the ``EMOBILITY_BOOT_NOTIFICATIONS`` item as below, we can clearly see here the ``TS`` column has the ``STRING`` type.


![image039](../Images/image095.jpg)

<br>

Now select the ``target`` data set as below and verify the information in the  ``System Artifact Summary`` pane, and verify the ``TS`` column's ``type`` to be the desired ``DATETIME`` type. 

![image039](../Images/image096.jpg)

Lineage analysis helps to view and navigate through various dependencies between objects. For example, if you have some data that has been transformed or enhanced, you can find where the data originated to learn how the dataset could have been modified.

<br>

:clap: **Congratulations you have completed this introduction!** :clap:




<br>

## Learn more

If you want to learn more, we provide references containing further information:

- *Discover*
    - [Self-Service Data Preparation Guide for SAP Data Intelligence Cloud](https://help.sap.com/viewer/305fdeeaf7e84ff38cfeff576184472c/Cloud/en-US/55cd5863c69d4d9eab2f2b886e909273.html?q=data%20preparation)
    - [SAP Data Intelligence Cloud ](https://www.sap.com/products/database-data-management.html?pdf-asset=084f548e-847d-0010-87a3-c30de2ffd8ff&page=1)
    - [Analyze Data Lineage](https://help.sap.com/viewer/1840b1ec6f774cd89a0fe7129910ecd3/Cloud/en-US/873e20623b904f7c8eee49ddb11498a2.html)
  
- *Watch*
    - [Self-Service Data Preparation](https://www.youtube.com/watch?v=3-V8qQWkHvk)
    - [SAP HANA Academy Videos - Data Intelligence Cloud](https://www.youtube.com/watch?v=2tC4GBUjxuc)
- *Read*
    - [SAP’s Unified Data and Analytics Solution Brief](https://www.sap.com/programs/data-analytics.html?pdf-asset=6e782098-ec7d-0010-bca6-c68f7e60039b&page=1)
- *Dive*
    - [SAP Data Intelligence | Hands-on Video Tutorials](https://blogs.sap.com/2021/02/04/sap-data-intelligence-hands-on-video-tutorials/)
    - [Build Your First Pipeline with SAP Data Intelligence, trial edition](https://developers.sap.com/group.dataintelligence-trial-2-pipelines.html)

[Exercise 2.0 Data Modeling with Data Warehouse Cloud](../ex2/Introduction_and_prerequisites.md) 

- - - -
