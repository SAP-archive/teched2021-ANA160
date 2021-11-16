# Exercise 2.5 - Spatial Reference

In this exercise we will build a dimension view with Spatial Reference and associate it with E_mobility-Teched view built in exercise 4.

At the conclusion of this exercise your Graphical View will look similar to the image below

![](Images/spatialreferenceimage/image27.png)





Click on Close button to go back to the DataBuilder

![](Images/spatialreferenceimage/image1.png)

Click on the New Graphical View option in the Data Builder.

![](Images/spatialreferenceimage/image2.png)

To import the data from 'Hana Cloud' navigate to the Sources tab and find the TechEd_HC connection under the Connections. Under **TechEd_HC** Connection drill down on **ANA160**

 Under **ANA160** drill down on **Views** and select **EMOBILITY_LIVE_CHARGE_STATUS**(table) Drag and drop the table in to Canvas

(Drill down flow Connections -\> TechEd_HC -\> ANA160-\> Views-\> EMOBILITY_LIVE_CHARGE_STATUS)

![](Images/spatialreferenceimage/image3.png)

Click on **Import and Deploy**

![](Images/spatialreferenceimage/image28.png)

Click on Output View

![](Images/spatialreferenceimage/image4.png)

Change Semantic Usage from "Relational Dataset" to "Dimension".

![](Images/spatialreferenceimage/image5.png)

Click on the "EMOBILITY_LIVE_CHARGE_STATUS" view to open the context menu

Click on 'fx'(Calculated Columns).

![](Images/spatialreferenceimage/image6.png)

Click on the **+** icon and select Geo-Coordinates Column

![](Images/spatialreferenceimage/image7.png)

Select Latitude as **LAT**

![](Images/spatialreferenceimage/image8.png)

Select Longitude as **LONG**

![](Images/spatialreferenceimage/image9.png)

Click on Output View

And change the Business Name as **E_mobility_location**

Technical Name as **Location**

Set the Expose for Consumption to 'ON'

![](Images/spatialreferenceimage/image10.png)

Click on Save, again on Save and then Deploy.

![](Images/spatialreferenceimage/image11.png)

See that Dimension View has been Deployed

![](Images/spatialreferenceimage/image12.png)

From the context menu of E_mobility_location select **Preview** to see the data.

![](Images/spatialreferenceimage/image13.png)

Click on Close button and Go to DataBuilder

![](Images/spatialreferenceimage/image14.png)

Click on the view **E_mobility-Teched**

![](Images/spatialreferenceimage/image15.png)

Scroll down to add the Associations.

![](Images/spatialreferenceimage/image16.png)

Click on the **+** icon to select the Association.

![](Images/spatialreferenceimage/image17.png)

Click on Association

![](Images/spatialreferenceimage/image18.png)

Search for View (Dimension) **E_mobility_location**

![](Images/spatialreferenceimage/image19.png)

Select that View and click on "OK"

![](Images/spatialreferenceimage/image20.png)

See the Mappings between both the Views.

![](Images/spatialreferenceimage/image21.png)

Click on ![](Images/spatialreferenceimage/image22.png)

![](Images/spatialreferenceimage/image23.png)

We can see the associations in the **E_mobility-Teched** view

![](Images/spatialreferenceimage/image24.png)

From the context menu of  **E_mobility-Teched** select **Preview data** to see the data.

![](Images/spatialreferenceimage/image25.png)

Click on **Deploy** to update the changes.

![](Images/spatialreferenceimage/image26.png)

Congratulations on completing all SAP DataWarehouse Cloud related exercises.

In the next section we would be consuming the view in SAP Analytics Cloud to analyse and get insights from data.

[Exercise 3 Building dashboards with SAP Analytics Cloud](../ex3/1.Introduction_and_Log_in.md)