# Egeria Semantics workgroup 20th of February

## Agenda:
* Daniela presented on metadata driven security 
* AOB 

## Attendees:
* David Radley (IBM)
* Mandy Chessell (IBM)
* Pat O'Sullivan (IBM)
* Daniela Otelea (ING)



## Minutes:

* Daniela presented on metadata driven security 
    * Daniela talked of the first phase of metadata driven security being Ranger, Active directory and Gaian
    * The second phase will be "full integration" including security officer and showing the use of the security tags confidentiality and subject area. 
    Mandy thought that origin (country)  might be in scope as well, as we had previously included origin in these simpler use cases.
   * We talked about the definitiion of subjkect area, there as an IGC logical model definition that was not the Egeria subject area. Daniela is using IGC
   for this proof point so needs to find how the subject area classification is represented in IGC and exposed through the IGC proxy.
   * We talked about some of the history. An employee with a work address and a home address both in the Employee subject area.
* We talked about the nature of subject area. How granular should it be , Mandy suggested that the granularity would be dictated by
   the organizational structure; if the subject area experts are expert in a fine grained area this could be a subject area. Other organizations may require
    courser subject areas. 
* Mandy said that Egeria subject area classification is now not just applicable to a GlossaryCategory, it is on Referenceable. Maybe subject area could 
be specified in a similar way to Zones; with definitions in area 4 and in classifications.        
* Pat talked of 2 types of subject area
    * core subject area concepts like Party and Project 
    * particular vernacular for a particular business
* Pat talked to of industry models being consumed in 2 different ways 
    * as is 
    * as inspiration for an organisations models. 
* Pat asked about zones; thinking about zones on glossary terms. Mandy confirmed that in Egeria zones are only against assets.
                   
* We talked of the Subject Area including not just the glossary but also the logical model, reference data and rules
## Actions:
* Daniella to workout the simplest glossary structure that could be used to show the subject area influencing security authorization. For example
a Glossary Term could have more than one category, but it should only be in one subject area.
* Daniella to confirm the IGC mappings of content to Egeria concepts via the project is as she would expect.    
## Next session:
Working session to map model constructs (for example owl, rdf, rdfs namespace elements) to Egeria types 
(mostly in area 3 starting with GlossaryTerms and Term to Term relationships ) 