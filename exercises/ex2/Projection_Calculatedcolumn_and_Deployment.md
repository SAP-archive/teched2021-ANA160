

# Exercise 4: Projection, Formulas and View deployment



In this exercise we will introduce a projection to exclude columns, include a formula and deploy the view.

At the conclusion of this exercise your Graphical View will look similar to the image below

![](Images/Projection_Calculatedcolumn_and_Deployment/image26.png)



#### **Add a Projection**

1.  Click on the Join
2.  In the context click on **Rename/Exclude Columns (Projection)**

![](Images/Projection_Calculatedcolumn_and_Deployment/image1.png)

3. Click on ![](Images/Projection_Calculatedcolumn_and_Deployment/image2.png) to Exclude TS Column.

> ![](Images/Projection_Calculatedcolumn_and_Deployment/image3.png)

4. Click on Exclude Column.

![](Images/Projection_Calculatedcolumn_and_Deployment/image4.png)

![](Images/Projection_Calculatedcolumn_and_Deployment/image5.png)

5.Click on the **Projection**

6Click on the **Calculated Columns** from the context

![](Images/Projection_Calculatedcolumn_and_Deployment/image6.png)

7. Properties panel of the **fx** node is displayed

![](Images/Projection_Calculatedcolumn_and_Deployment/image7.png)

8. Click on the + icon to add a column

![](Images/Projection_Calculatedcolumn_and_Deployment/image8.png)

9. Click into the Expression box and type:

10. STOPROUNDEDPRICE/1000

11. Then, click Validate.

![](Images/Projection_Calculatedcolumn_and_Deployment/image9.png)

12. Change the Business Name as **Cost** and Technical Name as **Cost** for the Calculated Column

![](Images/Projection_Calculatedcolumn_and_Deployment/image10.png)

13. Click on Columns

![](Images/Projection_Calculatedcolumn_and_Deployment/image11.png)

14. Click on the Data Preview icon to see the newly added Calculated Column(**Cost)** data.

![](Images/Projection_Calculatedcolumn_and_Deployment/image12.png)

15. If we don't find the column in the preview, click on Column Settings, search for **Cost** then select **Cost** column from the list and Click OK.

![](Images/Projection_Calculatedcolumn_and_Deployment/image13.png)

![](Images/Projection_Calculatedcolumn_and_Deployment/image14.png)

16. Click on Data Preview.

![](Images/Projection_Calculatedcolumn_and_Deployment/image15.png)

17. Click on **View1** to change the View properties.

![](Images/Projection_Calculatedcolumn_and_Deployment/image16.png)

18. Do the following changes to the Properties of the View:

19. Enter Business Name as **E_mobility-Teched**

20. Enter the Technical Name as **E_mobility-Teched**

![](Images/Projection_Calculatedcolumn_and_Deployment/image17.png)

21.Change Semantic Usage from "Relational Dataset" to "Analytical Dataset".

![](Images/Projection_Calculatedcolumn_and_Deployment/image18.png)

22. Set "Expose for Consumption" to ON

23. Setting "Expose for Consumption" makes the artifact available for consumption in the SAP Analytics Cloud for Story Building (Analytical Dataset Views only) and other analytical clients.

![](Images/Projection_Calculatedcolumn_and_Deployment/image19.png)

24. We are now going to select the measures

25. Can use the search bar to find the measures

26. With Control key pressed + Left mouse click on "STOPTOTALINACTIVITYSECS","STOPPRICE","STOPROUNDEDPRICE","Cost"

27. Click on the 3 dots (...)

28. Click on "Change to Measure".

> **OR** you can click on the "STOPTOTALINACTIVITYSEC", "STOPPRICE" "STOPROUNDEDPRICE","Cost" for each of the attributes and select **Change to Measure**.

![](Images/Projection_Calculatedcolumn_and_Deployment/image20.png)

29. Click on Save

![](Images/Projection_Calculatedcolumn_and_Deployment/image21.png)

30. Click on Save

![](Images/Projection_Calculatedcolumn_and_Deployment/image22.png)

32. Now you can "Deploy" the Data Model.

33. Click "Deploy".

![](Images/Projection_Calculatedcolumn_and_Deployment/image23.png)

34. Check the Deployed status

![](Images/Projection_Calculatedcolumn_and_Deployment/image24.png)

35. Click on the output data set 'E_mobility-Teched'

36. From the context click on Data Preview to see the data.

![](Images/Projection_Calculatedcolumn_and_Deployment/image25.png)

[Exercise 5. Spatial Reference](../ex2/Spatial_reference.md)