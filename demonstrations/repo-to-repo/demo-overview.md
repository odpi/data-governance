<!-- SPDX-License-Identifier: CC-BY-4.0 -->
<!-- Copyright Contributors to the ODPi Egeria project. -->

# OMRS Repository-to-Repository Demonstration

## Objective:   		

To illustrate metadata sharing between repositories and support both a "technical" and "business benefits" viewpoint.  
Requirements:	At a high level, this demo will be an asset that supports live and recorded demos, with the potential to be repeated in downloadable vm's or in a cloud demo environment (licensing issues to be determined, and will probably depend on eventually having multiple versions of this demo ....Atlas - Atlas, IGC - IGC, IGC - Atlas, etc).  The demo has to be brief and illustrate bi-directional sharing of technical and business metadata.   Demo (for a recording) needs to be less than ten minutes in length, preferably less than 6 or 8.   "In person" live demos can be longer and dive deeper.

## Source:		

Per last week's meeting, and David's suggestion, artifacts and storyboard will be inspired by the ODPi Egeria Privacy Pack and also Coco Pharmaceuticals.

## Capabilities:		

OMRS is limited at this point in its early release to RDBMS and Business Term artifacts.  This demo will focus on the sharing of newly ingested database tables and columns, newly created and existing business terms, and their assignment to a database table and/or column(s).  However, as OMRS matures, other metadata types and relationships can be added. 


## Demo Scenario

The script describes two persona that are important to GDPR and Data Privacy Management.    An "Asset Owner" and a "Data Privacy Officer".    They will be described  as working at Coco Pharmaceuticals (see other links in the project, such as https://github.com/odpi/data-governance/tree/main/data-privacy-pack and https://github.com/odpi/data-governance/tree/main/docs/coco-pharmaceuticals), where the Data Privacy Officer is responsible for evaluating new systems and application offerings, setting privacy policies, and leading data privacy assessments, and the Asset Owner being someone with responsibility/ownership/management of a new offering for customers/new business, etc. [proposed participants for the demo script will be "Faith" (Data Privacy Officer) and then Erin, Tessa and Jules, as team members with architecture or data steward responsibility surrounding clinical research]. The demo script won't have time to go into deep detail on their roles, but will establish their positions and responsibilities. The Asset Owner is part of a team that is proposing and building, or soon to deploy, a mobile clinical trials application for monitoring drug use.   Before the application can be approved, it must first be reviewed by the Data Privacy team.   How extensive that review is, and whether a detailed Privacy Impact Assessment must be scheduled, is the responsibility of the Data Privacy Officer.  

[Note:  depending on the "current" level of metadata sharing support among OMRS Connector implementations, the demo script might start with the creation and sharing of a Business Term, or perhaps the creation and sharing of the metadata for a relational table, but ultimately the goal is to illustrate bi-directional sharing of "new" metadata and then also the "assignment" of terminology to a particular data asset....but the exact "order" of creation/sharing may vary from the script described below based on what amount of functionality is available ---- particularly for an initial demo implementation targeted for Vancouver North America Summit (August, 2018).]

The new application is being developed in the team's "favorite tooling" or platform --- one that already supports OMRS --- or is being modeled using resources or an application that is already supported by Apache Atlas (Hive, Business Terms as modeled in Apache Atlas, etc.).     The Asset Owner decides that the metadata for the new application has reached a point of stability and is ready for review by the corporate Privacy Team.   This metadata content includes a set of tables, several of which contain columns that can be qualified as "Personal Data" (some account information, name details, ip and other mobile information, etc.).   Some of the metadata is tagged by Business Terms related to the privacy effort.    The Asset Owner "enables" sharing with the central repository that is the corporate preferred repository for all governance activities, and is monitored by the Data Privacy Officer and others on their team ("enables" means kicking off the process to force first-time metadata sharing --- this might be a new import, publication of Terms, running a script, or other similar action that starts the OMRS Connector).  

Our Data Privacy Officer receives a notification that new metadata is "available for review".  They are then able to see the new metadata, in the central repository tooling, which includes database table and column information, along with several business Terms that classify columns as "Personal Data".     It looks good, but needs further qualification at the table level for some of the database tables, whose status for privacy is elevated to a higher level due to a "combination" of columns recognized as critical for privacy by the company when they co-exist in the same dataset.   The Data Privacy Officer starts the process to schedule time for a thorough Privacy Impact Assessment of the new application, and submits the metadata change at the table level for immediate review by the application owners.    The demo concludes when the Asset Owner receives confirmation that an initial review has taken place, and is also able to immediately see that additional tagging of their resources has been performed by the Data Privacy team.   

From a technical perspective, the demo illustrates automated and real-time sharing of metadata between the two repositories, in both directions.  The expectation is that the traffic between repositories will be illustrated by opening a window to one or more kafka-consumers.   This helps describe the technical parts of the solution, as well as emphasis the "real-time" automation happening behind the scenes.  This will also help address the needs of different audiences for this demo, whether they are developers or users, and with a technical or governance/business background.

----
License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/),
Copyright Contributors to the ODPi Egeria project.
