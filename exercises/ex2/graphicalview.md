

### Exercise 2: Create Graphical View 

We will create our model in an intuitive graphical interface and at the conclusion of this exercise your Graphical View will look similar to the image below

![](Images/Graphicalview/image10.PNG)

We will continue to enhance the view as we progress through the exercises.

## Data Builder

1.  To expand the navigation menu click on ![](Images/Graphicalview/image1.png) (Click on the lines in the top left corner, you'll see the full list of features)

![](Images/Graphicalview/image2.png)

![](Images/Graphicalview/image3.png)

2.  To start building Data Models click on "Data Builder".

3.  Now select the space in which you are going to work. In our demo click on the Space **TECHED2021**

![](Images/Graphicalview/image4.png)

![](Images/Graphicalview/image5.png)

4.  You can now create a graphical view using the data source from the connection already created. Click on the New Graphical View option in the Data Builder.

![](Images/Graphicalview/image6.png)

5.  To import the data from "Hana Cloud" navigate to the Sources tab and find the **TechEd_HC** connection under Connections. Drill down **TechEd_HC** Connection, drill down on **AC3538U01**
6.  Drill down **Views**, select **EMOBILITY_STATION_DATA**(table).
7.  Drag and drop the table (**EMOBILITY_STATION_DATA)**on to the canvas.
  
  (Drill down flow :**Connections -\> TechEd_HC -\> AC3538U01-\> Views-\> EMOBILITY_STATION_DATA**)

![](Images/Graphicalview/image7.png)


![](Images/Graphicalview/image8.png)

8.  To import the data from S/4HANA navigate to the Sources tab and find the **teched_HE4** connection under Connections. Drill down **teched_HE4** Connection, drill down **ABAP Tables by table name**, drill down on "**Z**", drill down on "**ZE**" and choose **ZEMOBILITYUSERS**

Drilldown flow :  (**Connections** -\> **teched_HE4** -\> **ABAP Tables by table name** -\> **Z** -\>**ZE** -\> **ZEMOBILITYUSERS**)

**Note**: "teched_HE4" which is connecting to S/4Hana system.

![](Images/Graphicalview/image9.png)

9.  Drag and drop the table(ZEMOBILITYUSERS) right on top of the "EMOBILITY_STATION_DATA" table and click on JOIN in the pop-up.

![](Images/Graphicalview/image11.png)
