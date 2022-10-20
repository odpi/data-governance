# Egeria Semantics workgroup 6th of February

## Agenda:
* introduction and big picture
* initial activities
   * subject area OMAS
   * json-ld and Michal's work
   * future meeting, agree when and how often.  
   * AOB 

## Attendees:
* David Radley
* Graham Wallis
* Michal Miklas


## Minutes:
* we introduced ourselves and what we are looking for from this workgroup
* David is interested in semantic models and wants to share , publicise, improve the subject area omas, see how Egeria can consume model content and how this is visualised for different personals in Egeria .
* Michal is interested in using Egeria as a way to get the IBM industry models to new audiences by having the IBM industry models in an open format that Egeria can take in. Michal talked of models moving from being ER models to the glossary terms being the primary artifact to encapsulate enterprise knowledge. Logical models and glossaries together give an ontology. He is trying to capture glossaries in an ontological way. He would like to view metadata like a graph db, utilizing schema content. He has experience of attempting to visualize glossary content. We talked about Egeria needing to have the capability to take licensed model content -(David observation - this probably means Egeria stores the license with the model elements and glossary terms).          
* Michal asked what was a SubjectArea ( by this he meant the Egeria type SubjectArea - which is a classification of a category ). David said he would supply a link to the Coco Pharmaceuticals use case sround subject areas - this is here https://github.com/odpi/data-governance/blob/main/docs/coco-pharmaceuticals/scenarios/defining-subject-areas/README.md
* We talked about how Apache Atlas implemented glossary content and how that can be brought into Egeria using a read only connector.
* David described the subject area OMAS , what is does and how it differs from Apache Atlas.
* We then discussed 2 UI capabilities relevant to semantics and models. The first is TEX (coded) to explore the Egeria type system and REX (work in progress) an OMRS D3 visualisation to facilitate metadata exploration using a combination of full text search , filters and graph navigation. The REX UI was not for a business user, but was useful for education, demos, diagnostics of a cohort. The 2nd UI capability is to take this UI component and reuse and extend it on top of an OMAS API to expose a persona / business oriented version of this metadata explorer.
* Michal talked of the format to use to store the ontology. He talked of the CIM model (https://cloudinformationmodel.org/) and compared its format with https://schema.org/ and the gs1 extension http://blog.schema.org/2016/02/gs1-milestone-first-schemaorg-external.html. Michal talked of some of the pros and cons of these models and had some thoughts around the open formats he would like to see Egeria consume. He agreed to present his understanding and assessment of these formats and some propose some requirements on Egeria in this area. Michal will do this in the next session.

## Next session:
Due to Michal's availability we will run the next session on Thursday the 20th of February 3PM UK time and weekly after that. If this time is not working for you - let me know and I will try to find a better slot. .
Michal to present assessment of model formats and propose options that would be useful for Egeria to adopt - so we can discuss and get consensus.    
         
I am looking at putting these minutes on the data governance website.
