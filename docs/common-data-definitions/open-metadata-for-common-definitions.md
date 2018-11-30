<!-- SPDX-License-Identifier: CC-BY-4.0 -->
<!-- Copyright Contributors to the ODPi Data Governance project. -->

# Open metadata for common data definitions

The [ODPi Egeria project](https://odpi.github.io/egeria/) provides a comprehensive set of
[open metadata types](https://odpi.github.io/egeria/open-metadata-publication/website/open-metadata-types/)
for managing [common data definitions](README.md).  These types provide a common language and format for exchanging
these definitions between tools and metadata repositories.  Each tool/repository provides a mapping to the ODPi Egeria types
and Egeria manages the exchange of metadata between these parties.

## The glossary

The glossary is at the heart of the common data definitions.
Figure 1 shows that the glossary contains glossary terms.  Each glossary term describes a concept used by the business.
It is also possible to link two glossary terms together with a relationship.
The relationship may describe a semantic relationship or a structural one.

![Figure 1](semantic-to-implementation-glossaries.png)
> Figure 1: Glossaries for describing concepts and the relationships between them

See [anatomy of a glossary](anatomy-of-a-glossary.md) for more information about creating glossaries.

## Data classes

Data classes provide definitions of
 * Logical types
 * How to detect them in data
 * Preferred implementation types for different technologies

Data classes can be linked together in part-of and is-a hierarchies.  For example,
Date, Social Security Number, Credit Card Number.

Each data class is linked glossary terms to show how data with that meaning should be represented.
This helps to create a candidate list for glossary term assignment recommendations based on
the data values stored if they can be matched to a data class.

![Figure 2](semantic-to-implementation-data-classes.png)
> Figure 2: Data classes for describing the logical data types and implementation options

## Schemas

![Figure 3](semantic-to-implementation-schemas.png)
> Figure 3: Schemas for documenting the structure of data

## Schemas and assets

![Figure 4](semantic-to-implementation-assets-and-schemas.png)
> Figure 4: Assets for documenting the organization's important data assets

## Connectors and connections

![Figure 5](semantic-to-implementation-connectors.png)
> Figure 5: Connection information needed to access the data held by an asset

## Metadata discovery

A discovery engine is a process that runs a pipeline of analytics to describe the data content of an asset.
It uses statistical analysis, reference data and other techniques to determine the type and range of values stored,
potentially what the data means and its level of quality.
The result of the analysis is stored in metadata objects called annotations.

![Figure 6](semantic-to-implementation-discovery.png)
> Figure 6: Output from a metadata discovery engine

## Bringing it all together

Figure 7 shows each of these pieces linking together.
In a real-world environment, the aim is to automate as much of this linkage as possible.
This is made considerably easier if the implementation landscape is reasonable
consistent.  However, where the stored data values do not match the expected types defined in the
schema, the metadata model reveals the inconsistencies and often requires human intervention to
ensure the links are correct.

![Figure 7](semantic-to-implementation-big-picture.png)
> Figure 7: Linking the metadata together



----
License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/),
Copyright Contributors to the ODPi Data Governance project.
