# Exercise 0 - Architecture and Overview

In this exercise you will learn about the architecture implemented in this hands-on workshop.

## 0 - Workshop Architecture

<br>

![](/exercises/Images/arch.jpg)

<br>

<!-- ## Exercise 0.2 - SAP Data Intelligence -->
## 0.1 - REST API integration SAP Data Intelligence 

SAP Data Intelligence graph is a network of operators connected to each other using typed input ports and output ports for data transfer where users can define and configure the operators in a graph.

In our hands-on workshop we have used the custom Python Operator with custom eMobility API calls to consume and transform API data that are staged in SAP Hana Cloud.

The workshop is not focused on Data Pipelining and consumption, this is merely background information on data origin.

<br>

Data Intelligence Launchpad is a central access point for various tool sets with in the Data Intelligence Suite. The Modeler is the tool set used to create Graphs (Data Pipelines).

![](/exercises/Images/mod_1.jpg)

Customizable Python operator with custom API calls and data transformation.

![](/exercises/Images/mod_2.jpg)

Example of eMobility API call with standard Python requests.

![](/exercises/Images/mod_3.jpg)


SAP Hana Cloud Operator configuration attributes.

![](/exercises/Images/mod_4.jpg)



<!-- ## Exercise 0.3 - SAP Data Warehouse Cloud -->
## 0.2 - S/4 User Metadata Integration

Description of DWC role in the overall solution/workshop... ... outcome of hands-on

## 0.3 - Model data in Data Warehouse Cloud
 


...


## 0.4 - Data Federation

eMobility historical data is loaded into the Data lake via a Data Intelligence Cloud Graph (Pipeline). The historical data is then federated by creating virtual tables via Database Explorer as seen in the image below.

This give us the ability to join the historical data with more recent hot data resident in SAP HANA Cloud for analysis.

<br>


![](/exercises/Images/fed.jpg)

Data lake is an SAP HANA Cloud component composed of data lake IQ – which provides high-performance analysis for petabyte volumes of relational data – and data lake Files – which provides managed access to structured, semistructured, and unstructured data stored as files in the data lake.

Data lake is fully integrated into SAP HANA Cloud, sharing common security and tooling.

Data lake is available in different configurations. You can integrate it into a SAP HANA Cloud, SAP HANA database instance, or you can provision a standalone data lake instance with no SAP HANA database integration. You can also enable or disable the data lake IQ component when provisioning your data lake instance.

## 0.5 - Build Dashboards in SAP Analytics Cloud


 .....

Description of SAC role in the overall solution/workshop... outcome of hands-on


<br>![](/exercises/ex0/images/subscribe_webide.png)




## Summary

We are now fully set up and can start with the actual hands on exercise. In the very next step, we will upload the demo project, to have an environment with data.

Continue to - [Exercise 1 - Self-Service Data Preparation with Data Intelligence](../ex1/README.md)