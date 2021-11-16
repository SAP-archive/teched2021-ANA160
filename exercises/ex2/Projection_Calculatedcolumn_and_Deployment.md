

# Exercise 2.4 - Projection, Formulas and View deployment



In this exercise we will introduce a projection to exclude columns, include a formula and deploy the view.

At the conclusion of this exercise your Graphical View will look similar to the image below

![](Images/Projection_Calculatedcolumn_and_Deployment/image26.png)



#### **Add a Projection**

Click on the Join
In the context click on **Rename/Exclude Columns (Projection)**

![](Images/Projection_Calculatedcolumn_and_Deployment/image1.png)

Navigate to TS column. Click on TS and then click on ![](Images/Projection_Calculatedcolumn_and_Deployment/image2.png) to Exclude TS Column.

> ![](Images/Projection_Calculatedcolumn_and_Deployment/image3.png)

Click on Exclude Column.

![](Images/Projection_Calculatedcolumn_and_Deployment/image4.png)

![](Images/Projection_Calculatedcolumn_and_Deployment/image5.png)

Click on the **Projection**

Click on **'fx'(Calculated Columns)** from the context.

![](Images/Projection_Calculatedcolumn_and_Deployment/image6.png)

Properties panel of the **fx** node is displayed

![](Images/Projection_Calculatedcolumn_and_Deployment/image7.png)

Click on the + icon to add a column

![](Images/Projection_Calculatedcolumn_and_Deployment/image8.png)

Click into the Expression box and type STOPROUNDEDPRICE/1000

Then, click Validate.
Note: If the default Data Type is set to String, change it to Double.

![](Images/Projection_Calculatedcolumn_and_Deployment/image9.png)

Change both the Business Name and Technical Name to **Cost** for the Calculated Column

![](Images/Projection_Calculatedcolumn_and_Deployment/image10.png)

Click on Columns

![](Images/Projection_Calculatedcolumn_and_Deployment/image11.png)

Click on the Data Preview icon to see the newly added Calculated Column(**Cost)** data.

![](Images/Projection_Calculatedcolumn_and_Deployment/image12.png)

If we don't find the column in the preview, click on Column Settings, search for **Cost** then select **Cost** column from the list and Click OK.

![](Images/Projection_Calculatedcolumn_and_Deployment/image13.png)

![](Images/Projection_Calculatedcolumn_and_Deployment/image14.png)

Click on Data Preview. You may need to scroll to the right to see the Cost column appear in the preview.

![](Images/Projection_Calculatedcolumn_and_Deployment/image15.png)

Click on **View1** to change the View properties.

![](Images/Projection_Calculatedcolumn_and_Deployment/image16.png)

Do the following changes to the Properties of the View:

Enter Business Name as **E_mobility-Teched**

Enter the Technical Name as **E_mobility-Teched**

![](Images/Projection_Calculatedcolumn_and_Deployment/image17.png)

Change Semantic Usage from "Relational Dataset" to "Analytical Dataset".

![](Images/Projection_Calculatedcolumn_and_Deployment/image18.png)

Set "Expose for Consumption" to ON

Setting "Expose for Consumption" makes the artifact available for consumption in the SAP Analytics Cloud for Story Building (Analytical Dataset Views only) and other analytical clients.

![](Images/Projection_Calculatedcolumn_and_Deployment/image19.png)

Now we are going to select some measures

We can use the search bar to find our measures or scroll down within the Attributes section.

Use control key + Left mouse click on "STOPTOTALINACTIVITYSECS","STOPPRICE","STOPROUNDEDPRICE","Cost"

Click on the 3 dots (...)

Click on "Change to Measure".

> **OR** you can click on the "STOPTOTALINACTIVITYSECS", "STOPPRICE" "STOPROUNDEDPRICE","Cost" for each of the attributes and select **Change to Measure**.

![](Images/Projection_Calculatedcolumn_and_Deployment/image20.png)

Click on Save

![](Images/Projection_Calculatedcolumn_and_Deployment/image21.png)

Click on Save

![](Images/Projection_Calculatedcolumn_and_Deployment/image22.png)

Now you can "Deploy" the Data Model.

Click "Deploy".

![](Images/Projection_Calculatedcolumn_and_Deployment/image23.png)

Check the Deployed status

![](Images/Projection_Calculatedcolumn_and_Deployment/image24.png)

Click on the output data set 'E_mobility-Teched'

From the context click on Data Preview to see the data.

![](Images/Projection_Calculatedcolumn_and_Deployment/image25.png)

[Exercise 5. Spatial Reference](../ex2/Spatial_reference.md)