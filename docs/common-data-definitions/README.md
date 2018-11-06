<!-- SPDX-License-Identifier: CC-BY-4.0 -->
<!-- Copyright Contributors to the ODPi Data Governance project. -->

# Common data definitions

Common data definitions (also known as the common information model or CIM) create a shared understanding of data.
They are critical where data is to be shared between different systems and or groups of people.

Typically the common data definitions consist of:
* Names and descriptions for concepts described by the data.
* Semantic relationships between these concepts.
* Classifications of the concepts to indicate how they are used.
* Definitions of the valid data values for specific concepts.
* Preferred logical and physical data formats for storing data about these concepts.

The common data definitions are managed in a metadata catalog.  Governance classifications may be
added to these definitions wich in turn link to governance requirements.

Tools used by the organizaton to, for example, create new data stores, data visualizations, or APIs,
or analytics models are pre-populated with concrete data definitions by
automated tool bridges.
Each tool bridge extracts the relevant definitions from the metadata catalog, generates the concrete definitions
and loads them into the tool.  Where possible, these definitions inclue tags that link the definitions back to the
common data definitions.

When the new IT capablity is deployed to test and production environments, the tool typically produces a packaged
version of the concrete definitions with their tags that point to the metadata.
The dev-ops pipeline that deploys the artifact reads the tags and ensures that any specific governance requirements for
the specific type of data that is being used are met.
