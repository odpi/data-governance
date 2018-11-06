<!-- SPDX-License-Identifier: CC-BY-4.0 -->
<!-- Copyright Contributors to the ODPi Data Governance project. -->

# Building the governance team

When [Jules Keeper](../../personas/jules-keeper.md) joined Coco Pharmaceuticals as the CDO, he soon realized that the execution of
their business strategy to move to personalized medicine was being held back by their operational practices.
Some of this was related to their use and management of data (his responsibility to fix of course),
but there were broader issues relating
to security, IT infrastructure management, software development and their corporate governance.  He realizes
that he can not do this alone and calls his colleagues together to discuss how they proceed.

They agree to divide the work amongst themselves, using the traditional governance domains to divide out the
responsbilities, but maintaining the governance information using open metadata (Egeria) to be able to
coordinate their work across the governance domains.

The result is as follows:
* [Jules Keeper](../../personas/jules-keeper.md) becomes the CDO and head of the DATA governance domain.
* [Ivor Padlock](../../personas/ivor-padlock.md) becomes the CISO and head of the SECURITY governance domain.
* [Faith Broker](../../personas/faith-broker.md) becomes the CPO and head of the PRIVACY governance domain.
* [Reggie Mint](../../personas/reggie-mint.md) as the CFO becomes head of the CORPORATE governance domain.
* [Gary Geeke](../../personas/gary-geeke.md) as the infrastructure lead becomes head of the IT INFRASTRUCTURE governance domain.
* [Polly Tasker](../../personas/polly-tasker.md) as the most senior software manager becomes had of the SOFTWARE DEVELOPMENT governance domain.

[Erin Overview](../../personas/erin-overview.md) is also appointed the CDO for IT systems.
This makes her a deputy for Jules and recognizes her
role in ensure data is properly managed by IT.

ODPi Egeria includes a sample client
([docs](https://github.com/odpi/egeria/blob/master/open-metadata-resources/open-metadata-samples/access-services-samples/governance-program-client-samples/governance-leadership.md), 
[code](https://github.com/odpi/egeria/blob/master/open-metadata-resources/open-metadata-samples/access-services-samples/governance-program-client-samples/src/main/java/org/odpi/openmetadata/accessservices/governanceprogram/samples/GovernanceLeadershipSample.java))
that issues the appropriate API calls to set up this team through the
[Governance Program OMAS](https://github.com/odpi/egeria/blob/master/open-metadata-implementation/access-services/governance-program/README.md) Governance Leadership Interface.
