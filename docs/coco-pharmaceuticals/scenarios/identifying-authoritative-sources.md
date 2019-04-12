<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- Copyright Contributors to the ODPi Data Governance project. -->

# Identifying authoritative sources

An **authoritative source** can be throught of as the "best" source of a particular type of information.
Authoritative sources may come from trusted third parties or be explicitly identified and managed within the organization.

[Jules Keeper](../personas/jules-keeper.md) asks [Erin Overview](../persona/erin-overview.md) to work
with [Gary Geeke](../personas/gary-geeke.md) to build a list of authoritative sources for the business.

Erin and Gary have two resources to work with:

* Gary has a catalog of all of Coco Pharmaceutical's systems
* Erin has the [subject area definitions](defining-subject-areas.md)

For each subject area, they need to identify one or two systems that could
act as an authoritative source for that type of information.

They need to consider:

* Is this a strategic system that has a long term future?
* Is this system able to take on additional workload?
* Does this system support APIs and related mechanisms to allow it to supply data to other systems?
* Is this system kept up to date with regular feeds of information?
* Could this system support the work of a steward to resolve conflicts and fix values in the data?

The result of the excercise shows where there are critical gaps in the information landscape that need futher
investment.  This may be updates to the identified systems, or an investment in new systems.
The second is more likely in areas that are new for the business.  For example,
when Erin and Gary looked at the area of patient details they realized they do hold a lot of patient data
but it is locked in files received from the hospitals as part of each clinical trial.
Coco Pharmaceuticals has no capability to actively maintain information about the
patients they are treating through the personalized medicine services.

On the other hand, for employee data, they do have a single system for managing information about employees.
This also has the maintenance capabilities and is currently used to automatically update their LDAP (security)
directory.

----
License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/),
Copyright Contributors to the ODPi Data Governance project.
