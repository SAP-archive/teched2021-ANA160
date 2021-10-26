

# Exercise 5: Projections, Calculated columns and Deployment



In this exercise we will add a projection to exclude columns, introduce a calculated column and deploy the view.

At the conclusion of this exercise your Graphical View will look similar to the image below

![](Images/Projection_Calculatedcolumn_and_Deployment/image26.png)



#### **Add a Projection**

1.  Click on the Join
2.  In the context click on **Rename or Exclude Columns (Projection)**

![](Images/Projection_Calculatedcolumn_and_Deployment/image1.png)

1.  Click on ![](Images/Projection_Calculatedcolumn_and_Deployment/image2.png) to Exclude TS Column.

> ![](Images/Projection_Calculatedcolumn_and_Deployment/image3.png)

1.  Click on Exclude Column.

![](Images/Projection_Calculatedcolumn_and_Deployment/image4.png)

![](Images/Projection_Calculatedcolumn_and_Deployment/image5.png)

1.  Click on the **Projection**

2.  Click on the **Calculated Columns** from the context

![](Images/Projection_Calculatedcolumn_and_Deployment/image6.png)

1.  Properties panel of the **fx** node is displayed

![](Images/Projection_Calculatedcolumn_and_Deployment/image7.png)

1.  Click on the + icon to add a column

![](Images/Projection_Calculatedcolumn_and_Deployment/image8.png)

1.  Click into the Expression box and type:

2.  STOPROUNDEDPRICE/1000

3.  Then, click Validate.

![](Images/Projection_Calculatedcolumn_and_Deployment/image9.png)

1.  Change the Business Name as **Cost** and Technical Name as **Cost** for the Calculated Column

![](Images/Projection_Calculatedcolumn_and_Deployment/image10.png)

1.  Click on Columns

![](Images/Projection_Calculatedcolumn_and_Deployment/image11.png)

1.  Click on the Data Preview icon to see the newly added Calculated Column(**Cost)** data.

![](Images/Projection_Calculatedcolumn_and_Deployment/image12.png)

1.  If we don't find the column in the preview, click on Column Settings, then select **Cost** column from the list and Click OK.

![](Images/Projection_Calculatedcolumn_and_Deployment/image13.png)

![](Images/Projection_Calculatedcolumn_and_Deployment/image14.png)

1.  Click on Data Preview.

![](Images/Projection_Calculatedcolumn_and_Deployment/image15.png)

1.  Click on View to change the View properties.

![](Images/Projection_Calculatedcolumn_and_Deployment/image16.png)

1.  Do the following changes to the Properties of the View:
2.  Enter Business Name as **E_mobility-Teched**
3.  Enter the Technical Name as **E_mobility-Teched**

![](Images/Projection_Calculatedcolumn_and_Deployment/image17.png)

1.  Change Semantic Usage from "Relational Dataset" to "Analytical Dataset".

![](Images/Projection_Calculatedcolumn_and_Deployment/image18.png)

1.  Set "Expose for Consumption" to ON

2.  Setting "Expose for Consumption" makes the artifact available for consumption in the SAP Analytics Cloud for Story Building (Analytical Dataset Views only) and other analytical clients.

![](Images/Projection_Calculatedcolumn_and_Deployment/image19.png)

1.  We are now going to select the measures

2.  Can use the search bar to find the measures

3.  With Control key pressed + Left mouse click on "STOPTOTALINACTIVITYSECS","STOPPRICE","STOPROUNDEDPRICE","Cost"

4.  Click on the 3 dots (...)

5.  Click on "Change to Measure".

> **OR** you can click on the "STOPTOTALINACTIVITYSEC", "STOPPRICE" "STOPROUNDEDPRICE","Cost" for each of the attributes and select **Change to Measure**.

![](Images/Projection_Calculatedcolumn_and_Deployment/image20.png)

1.  Click on Save

![](Images/Projection_Calculatedcolumn_and_Deployment/image21.png)

1.  Click on Save

![](Images/Projection_Calculatedcolumn_and_Deployment/image22.png)

1.  Now you can "Deploy" the new Data Model.

2.  Click "Deploy".

![](Images/Projection_Calculatedcolumn_and_Deployment/image23.png)

1.  Check the Deployed status

![](Images/Projection_Calculatedcolumn_and_Deployment/image24.png)

1.  Click on the final data set 'E_mobility-Teched'

2.  From the context click on Data Preview to see the data.

![](Images/Projection_Calculatedcolumn_and_Deployment/image25.png)
