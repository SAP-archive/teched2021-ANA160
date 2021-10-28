# Exercise 5: Spatial Reference

In this exercise we will build a dimension view with Spatial Reference and associate it with E_mobility-Teched view built in exercise 4.

At the conclusion of this exercise your Graphical View will look similar to the image below

![](Images/spatialreferenceimage/image27.png)





1.  Click on Close button to go back to the DataBuilder

![](Images/spatialreferenceimage/image1.png)

1.  Click on the New Graphical View option in the Data Builder.

![](Images/spatialreferenceimage/image2.png)

1.  To import the data from 'Hana Cloud' navigate to the Sources tab and find the TechEd_HC connection under the Connections. Under **TechEd_HC** Connection drill down on **AC3538U01**

2.  Under **AC3538U01** drill down on **Views** and select **EMOBILITY_LIVE_CHARGE_STATUS**(table) Drag and drop the table in to Canvas

(Drill down flow Connections -\> TechEd_HC -\> AC3538U01-\> Views-\> EMOBILITY_LIVE_CHARGE_STATUS)

![](Images/spatialreferenceimage/image3.png)

1.  Click on Output View

![](Images/spatialreferenceimage/image4.png)

1.  Change Semantic Usage from "Relational Dataset" to "Dimension".

![](Images/spatialreferenceimage/image5.png)

1.  Click on the "EMOBILITY_LIVE_CHARGE_STATUS" view to open the context menu

2.  Click on "Calculated Columns".

![](Images/spatialreferenceimage/image6.png)

1.  Click on the **+** icon and select Geo-Coordinates Column

![](Images/spatialreferenceimage/image7.png)

1.  Select Latitude as **LAT**

![](Images/spatialreferenceimage/image8.png)

1.  Select Longitude as **LONG**

![](Images/spatialreferenceimage/image9.png)

1.  Click on Output View

2.  And change the Business Name as **E_mobility_location**

3.  Technical Name as **Location**

![](Images/spatialreferenceimage/image10.png)

1.  Click on Save, again on Save and then Deploy.

![](Images/spatialreferenceimage/image11.png)

1.  See that Dimension View has been Deployed

![](Images/spatialreferenceimage/image12.png)

1.  From the context menu of E_mobility_location select **Preview** to see the data.

![](Images/spatialreferenceimage/image13.png)

1.  Click on Close button and Go to DataBuilder

![](Images/spatialreferenceimage/image14.png)

1.  Click on the view **E_mobility-Teched**

![](Images/spatialreferenceimage/image15.png)

1.  Scroll down to add the Associations.

![](Images/spatialreferenceimage/image16.png)

1.  Click on the **+** icon to select the Association.

![](Images/spatialreferenceimage/image17.png)

1.  Click on Association

![](Images/spatialreferenceimage/image18.png)

1.  Search for View (Dimension) **E_mobility_location**

![](Images/spatialreferenceimage/image19.png)

1.  Select that View and click on "OK"

![](Images/spatialreferenceimage/image20.png)

1.  See the Mappings between both the Views.

![](Images/spatialreferenceimage/image21.png)

1.  Click on ![](Images/spatialreferenceimage/image22.png)

![](Images/spatialreferenceimage/image23.png)

1.  We can see the associations in the **E_mobility-Teched** view

![](Images/spatialreferenceimage/image24.png)

1.  From the context menu of  **E_mobility-Teched** select **Preview data** to see the data.

![](Images/spatialreferenceimage/image25.png)

1.  Click on **Deploy** to update the changes**.**

![](Images/spatialreferenceimage/image26.png)
