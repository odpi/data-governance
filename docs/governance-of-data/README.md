<!-- SPDX-License-Identifier: CC-BY-4.0 -->
<!-- Copyright Contributors to the ODPi Egeria project. -->

# Governance of data

Although ODPi Egeria supports all types of governance, it has a specific
focus on data governance because (1) data is so critical to modern digital business
and (2) data by its very nature needs special treatment.

Unlike a physical object, such as a chair or a building, data can be freely copied
and combined in multiple ways.  It is fluid.  This is why water analogies,
such as **data lake**, are popular when it comes to describing data management.

The fluidity of data creates 2 challenges:

* What are the dividing lines between different data assets?
* Who is responsible for the quality and protection of data when there are so many copies?

In addition, the original meaning of data is often lost.
Data is created in a specific context
(such as an application or from a specific sensor).
This context means there are certain assumptions made about the
precision, quality, timeliness and completeness of the data.

As the data is copied and sent to different destinations, this context
needs to be captured so it can be used to validate whether the data can be
used in a new context.

Some standard data formats, such as JPG and MP3 files, include support
for this context, which is called **metadata** (literally data about data).
However, most data is in a format that does not
include this metadata and it must be managed separately.

The next challenge is that people, in general, are sloppy about the precise meaning of the terminology they
use and this lack of precision can translate to misunderstandings on what specific data values mean.
Even within the same organization, a term may have multiple meanings,
or their may be multiple terms for the same thing.
In order the communicate the meaning of data from one context to another,
these anomalies in the meaning of the terminology used to describe the data need to
be reconciled.

Finally there is is still a lot of uncertainty related to ownership of data.
Just because an organization holds data, it does not mean it has the right to
process it.  The data may be subject to copyright (such as the
[Creative Commons licenses](https://creativecommons.org/licenses/),
or a more specific type of data license (such as the [Community Data License Agreement (CDLA)](https://cdla.io/)),
or may be personal data that is subject to specific data privacy regulations
(such as the [General Data Protection Regulation (GDPR)](https://ec.europa.eu/commission/priorities/justice-and-fundamental-rights/data-protection/2018-reform-eu-data-protection-rules_en)).

This means that the organization needs to track the flow of data between data stores and
applications to ensure that it is only used for approved purposes.
The organization needs to define the precise responsibilities of
people that hold copies of data and the requirements that they must fulfil.


----
Return to [Guidance on Governance](..).



----
License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/),
Copyright Contributors to the ODPi Egeria project.