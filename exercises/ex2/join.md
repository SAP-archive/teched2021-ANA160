# Exercise 2.3 -  Configuring Joins

In this exercise we will configure the join E-MOBILITY_STATION table with E-MOBILITY_USERS table.

At the conclusion of this exercise your Graphical View will look similar to the image below

![](Images/joinimage/image5.png)



## **Configuring Joins**

Click on the Inner Join box in the canvas, you'll see the JOIN PROPERTIES window on the right-hand side.

 Join Type - select **Left**.

> ![](Images/joinimage/image1.png)

 Cardinality needs to maintained for both tables. Click on ![](Images/joinimage/image2.png) and select Exactly One(1) for both tables

> ![](Images/joinimage/image3.png)
>
> ![](Images/joinimage/image4.png)

Join both the tables by using key record **User Id**

Drag and drop **USERID from E-Mobility Station Data table** on to **User Id present on E-Mobility users table**.

> ![](Images/joinimage/image5.png)

[Exercise 4. Projection and Formulas](../ex2/Projection_Calculatedcolumn_and_Deployment.md)
