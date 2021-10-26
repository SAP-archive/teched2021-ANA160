# DAT162 - Get the Most from Sensitive Data: SAP HANA Data Anonymization and Masking

<!-- [![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/teched2021-ANA160)](https://api.reuse.software/info/github.com/SAP-samples/teched2021-ANA160/) -->
<!-- 
## Description

TBA -->

## Overview

This repository contains the material for the SAP TechEd 2021 session called ANA160 - Give Data Purpose with SAP BTP and Cloud Analytics Solutions.

This session introduces attendees to the SAP data and analytics solutions in the cloud. You will get a hands-on experience of our flagship cloud solutions such as SAP Data Intelligence Cloud, SAP HANA Cloud, SAP Data Warehouse Cloud and SAP Analytics Cloud solutions.


## Use Case

Employees are increasingly using electrical vehicles as their choice of company car. That creates a challenge for companies to provide and manage charging infrastructure efficiently, by providing sufficient power to run the charging spots, manage any error-prone charging stations and incentives colleagues to charge at non-peak hours.


SAP solutions for new mobility like Charge Point Operations enable drivers, fleet, and facility managers to manage the vehicles, energy demand, charging infrastructure, and charging procedures. In this scenario you will get insights into:
- charging station consumption in SAP France two locations. Mougins and Caen in which we charge the e-Vehicles of our employees every day
- a real-time overview of the charging and suspended charging stations
- peak times along the day and during the week
- charging station usage of the employees

## Requirements

The requirements to follow the exercises in this repository are:
- SAP Data Intelligence tenant
- SAP SAC tenant
- SAP DWC tenant
Above requirements are already met, pre-created by SAP.

Instructions on how to start and use such trials are in [Exercise 0](exercises/ex0/).

## Exercises


- [Exercise 0 - Architecture and Overview](exercises/ex0/)
    - [Exercise 0.1 - Architecture](exercises/ex0#exercise-01---architecture)
    - [Exercise 0.2 - DI](exercises/ex0#exercise-02---sap-data-intelligence)
    - [Exercise 0.3 - DWC](exercises/ex0#exercise-03---sap-data-warehouse-cloud)
    - [Exercise 0.4 - SAC](exercises/ex0#exercise-04---sap-analytics-cloud)
    - [Exercise 0.5 - S/4](exercises/ex0#exercise-05---pull-user-data-from-sap-s/4)
 
- [Exercise 1 - Self-Service Data Preparation](exercises/ex1/)
    - [Exercise 1.1 - Introduction](exercises/ex1#exercise-11---introduction)
    - [Exercise 1.2 - Metadata Explorer](exercises/ex1#exercise-12---metadata-explorer)
    - [Exercise 1.3 - Browse Connections](exercises/ex1#exercise-13---browse-connections)
    - [Exercise 1.4 - Profile Data](exercises/ex1#exercise-14---profile-data)
    - [Exercise 1.5 - View Fact Sheet](exercises/ex1#exercise-15---view-fact-sheet)
    - [Exercise 1.6 - Prepare Dataset](exercises/ex1#exercise-16---prepare-dataset)
    - [Exercise 1.7 - Publish Dataset](exercises/ex1#exercise-17---publish-dataset)
- [Exercise 2 - DWC](exercises/ex2/)
    - [Exercise 2.1 - Introduction](exercises/ex2/Introduction_and_prerequisites.md)
    - [Exercise 2.2 - Logon to Data Ware House Cloud](exercises/ex2/LogOn_to_DWCimages.md)
    - [Exercise 2.3 - Creating a Graphical View](exercises/ex2/graphicalview.md)
    - [Exercise 2.4 - Creating a Join](exercises/ex2/join.md)
    - [Exercise 2.5 - Projection and Formulas](exercises/ex2/Projection_Calculatedcolumn_and_Deployment.md)
    - [Exercise 2.6 - Spatial](exercises/ex2/Spatial_reference.md)
- [Exercise 3 - SAC](exercises/ex3/)
    - [Exercise 3.1 - How can data be re-identified?](exercises/ex3/README.md#exercise-31---how-can-data-be-re-identified)
    - [Exercise 3.2 - Applying k-Anonymity](exercises/ex3/README.md#exercise-32---applying-k-anonymity)
    - [Exercise 3.3 - Showing the effects of k-Anonymity](exercises/ex3/README.md#exercise-33---showing-the-effects-of-k-anonymity)
    - [Exercise 3.4 - Evaluating a data science task on anonymized data](exercises/ex3/README.md#exercise-34---evaluating-a-data-science-task-on-anonymized-data)
    - [Exercise 3.5 - Applying Differential Privacy](exercises/ex3/README.md#exercise-35---applying-differential-privacy)


## Learn more

This exercise provides an overview about SAP HANA data masking and SAP HANA data anonymization. If you want to learn more, we provide references containing further information:

- *Discover*
    - [Self-Service Data Preparation Guide for SAP Data Intelligence](https://help.sap.com/viewer/305fdeeaf7e84ff38cfeff576184472c/Cloud/en-US)
    - [SAP Data Intelligence Cloud](https://help.sap.com/viewer/product/SAP_DATA_INTELLIGENCE/Cloud/en-US)

- *Watch*
    - [SAP HANA Academy Videos](https://www.youtube.com/watch?v=_iNJJw7AnrY)
    - [Expert Chat](https://www.youtube.com/watch?v=rePev1MfFdw)
- *Read*
    - [Privacy Protected Data Has Value Too!](https://blogs.sap.com/2019/07/10/privacy-protected-data-has-value-too-part-1-of-2/)
    - [Anonymize X+O Data](https://blogs.sap.com/2019/04/02/get-the-most-out-of-experiential-x-and-operational-o-data-with-sap-hana-real-time-data-anonymization/)
- *Dive*
    - [SAP Help: Anonymization Guide](https://help.sap.com/viewer/2f789e82e97d4f4e9416547abfbd012e/2020_03_QRC/en-US)
    - [Research paper (VLDB)](https://www.vldb.org/pvldb/vol12/p1998-kessler.pdf)
    - [SAP HANA Cloud Online Roadmap](https://roadmaps.sap.com/index.html#/board?categoryItems=73554900100800002881)
    - [SAP HANA Online Roadmap](https://roadmaps.sap.com/index.html#/board?categoryItems=01200314690800001945)

## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License
Copyright (c) 2020 SAP SE or an SAP affiliate company. All rights reserved. This file is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.