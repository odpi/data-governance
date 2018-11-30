<!-- SPDX-License-Identifier: CC-BY-4.0 -->
<!-- Copyright Contributors to the ODPi Data Governance project. -->

# Common data definitions

Common data definitions (also known as the common information model or CIM) create a shared understanding of data.
They are critical where data is to be shared between different systems and or groups of people.

Typically the common data definitions consist of:
* Names and descriptions for concepts described by the data.
* Relationships between these concepts.
* Classifications of the concepts to indicate how they are used.
* Definitions of the valid data values for specific concepts.
* Preferred logical and physical data formats for storing data about these concepts.

The common data definitions are managed in a metadata catalog.  The core definitions that cover the meaning of
data are described in one or more [glossaries](anatomy-of-a-glossary.md).

Governance classifications may be
added to these definitions which in turn link to governance requirements.   This determines how data that is
linked to these common definitions should be governed.

Tools used by the organizaton to, for example, create new data stores, data visualizations, or APIs,
or analytics models are pre-populated with concrete data definitions by
automated tool bridges.
Each tool bridge extracts the relevant definitions from the metadata catalog, generates the concrete definitions
and loads them into the tool.  Where possible, these definitions include tags that link the definitions back to the
common data definitions.

When the new IT capablity is deployed to test and production environments, the tool typically produces a packaged
version of the concrete definitions with their tags that point to the metadata.
The dev-ops pipeline that deploys the artifact reads the tags and ensures that any specific governance requirements for
the specific type of data that is being used are met.

Once the new capability is running, the IT infrastructure that is supporting it can be using the tags, and related metadata deployed to the production environment to manage the governance related to the capability, and, where the capability is also using metadata directly, to drive the function and data delivered to its consumer.

Figure 1 summarizes this process for using these common definitions.

![Figure 1](using-common-data-definitions.png)
> Figure 1: process for using common data definitions

The four boxes in figure 1 show the activity around managing the common definitions and below them are
the tools and processes using them.  Typically all 4 activities are running continually as the scope of the common
definitions typically starts small and expands as new projects consume them.

The **harvesting** activity is locating and extracting content for the common definitions from existing sources.
These may be definitions created by the organization for previous projects or definitions from external sources.
They need to be validated and and transformed so they can be injected into the catalog used to manage the definitions.

The **managing** activity describes the efforts of the subject matter experts to import, create and maintain the
common definitions in a catalog.  Typically the common definitions are organized into [subject areas](../coco-pharmaceuticals/scenarios/defining-subject-areas/README.md) (topics) and the appropriate subject matter experts are
assigned to each subject area.

The **consuming** activity is where the common definitions are transformed and made available in tools that are
being used to build or maintain new capability.

The **delivering value** activity is where the common definitions are beign used to deliver business function and
governance in the production systems.

## Further information

* [Open metadata for common data definitions](open-metadata-for-common-definitions.md)
* [Common Information Models for an open, analytical and agile world](http://www.ibmpressbooks.com/store/common-information-models-for-an-open-analytical-and-9780133366341)


----
License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/),
Copyright Contributors to the ODPi Data Governance project.
