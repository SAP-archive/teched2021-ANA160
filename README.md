# DAT162 - Get the Most from Sensitive Data: SAP HANA Data Anonymization and Masking

[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/teched2020-DAT162)](https://api.reuse.software/info/github.com/SAP-samples/teched2020-DAT162)

## Description

This repository contains the material for the SAP TechEd 2020 session called DAT162 - Get the Most from Sensitive Data: SAP HANA data anonymization and masking. 

## Overview

This session introduces attendees to the SAP HANA data masking and SAP HANA data anonymization functionality, by the running example of the company ACME. We will use SAP HANA Cloud, SAP HANA Cockpit and the SAP Web IDE. We will show how these features help to get the most out of the data, without risking the privacy of individuals.

Our example company ACME has, like any other company, a database of its employees containing, amongst other information, salaries and address information. There are multiple stakeholder personas within ACME that require access to the data, ranging from productive users, to data scientists:
- **HR Supervisor**: Has to be able to see and maintain any HR data.
- **HR Call Center agent**: Is of course allowed to see some details, e.g., when an employee calls and asks if the address is still correct. However, some information like the account number of an employee should be hidden so that this information cannot be leaked.
- **Data Scientist**: This persona requires access to analyze the HR data, e.g., how the payment structure of employees is. Of course, some data is required, but individual salaries must not be revealed.

Throughout this exercise we will use this as a running example.

## Requirements

The requirements to follow the exercises in this repository are:
- SAP HANA Cloud
- SAP Web IDE
Both are available as a trial, and this tutorial will focus on the trial version that it is accessible to anyone.

Instructions on how to start and use such trials are in [Exercise 0](exercises/ex0/).

## Exercises

- [Exercise 0 - Setting up the environment](exercises/ex0/)
    - [Exercise 0.1 - Creating a SAP Cloud Platform Trial Account](exercises/ex0#exercise-01---creating-a-sap-cloud-platform-trial-account)
    - [Exercise 0.2 - Creating a SAP HANA Cloud Trial Instance](exercises/ex0#exercise-02---creating-a-sap-hana-cloud-trial-instance)
    - [Exercise 0.3 - Creating the required users](exercises/ex0#exercise-03---creating-the-required-users)
    - [Exercise 0.4 - Creating a SAP Web IDE Trial Instance](exercises/ex0#exercise-04---creating-a-sap-web-ide-trial-account)
- [Exercise 1 - Meta Data Management](exercises/ex1/)
    - [1 - Introduction](exercises/ex1#1-introduction)
    - [2 - Metadata Explorer](exercises/ex1#2-metadata-explorer)
    - [Exercise 1.3 - Deploying the application to SAP HANA Cloud](exercises/ex1#exercise-13---deploying-the-application-to-sap-hana-cloud)
    - [Exercise 1.4 - Exploring the data](exercises/ex1#exercise-14---exploring-the-data)
    - [Exercise 1.5 - Understanding the demo scenario](exercises/ex1#exercise-15---understanding-the-demo-scenario)
- [Exercise 2 - Data Masking](exercises/ex2/)
    - [Exercise 2.1 - Configure and Deploy Data Masking via a SQL View](exercises/ex2#exercise-21---configure-and-deploy-data-masking-via-a-sql-view)
    - [Exercise 2.2 - Configure Privileged and Non-Privileged Roles for Access](exercises/ex2#exercise-22---configure-privileged-and-non-privileged-roles-for-access)
- [Exercise 3 - Data Anonymization](exercises/ex3/)
    - [Exercise 3.1 - How can data be re-identified?](exercises/ex3/README.md#exercise-31---how-can-data-be-re-identified)
    - [Exercise 3.2 - Applying k-Anonymity](exercises/ex3/README.md#exercise-32---applying-k-anonymity)
    - [Exercise 3.3 - Showing the effects of k-Anonymity](exercises/ex3/README.md#exercise-33---showing-the-effects-of-k-anonymity)
    - [Exercise 3.4 - Evaluating a data science task on anonymized data](exercises/ex3/README.md#exercise-34---evaluating-a-data-science-task-on-anonymized-data)
    - [Exercise 3.5 - Applying Differential Privacy](exercises/ex3/README.md#exercise-35---applying-differential-privacy)
- [Exercise 4 - Data Anonymization Report](exercises/ex4/)
    - [Exercise 4.1 - Accessing the anonymization reports](exercises/ex4#exercise-41---accessing-the-anonymization-reports)
    - [Exercise 4.2 - Understanding the report](exercises/ex4#exercise-42---understanding-the-report)

## Learn more

This exercise provides an overview about SAP HANA data masking and SAP HANA data anonymization. If you want to learn more, we provide references containing further information:

- *Discover*
    - [SAP HANA Security Website](https://www.sap.com/products/hana/features/security.html)
    - [SAP HANA data anonymization Website](https://www.sap.com/data-anonymization)
    - [Whitepaper](https://www.sap.com/documents/2016/06/3ea239ad-757c-0010-82c7-eda71af511fa.html)
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