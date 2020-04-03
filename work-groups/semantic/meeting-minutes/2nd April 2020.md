# Egeria Semantics workgroup 2nd of April 2020

## Agenda:
* Michal to present proposal of model formats and mappings from RDF to Egeria to IGC  

## Attendees:
* David Radley (IBM)
* Mandy Chessell (IBM)
* Michal Miklas (IBM)
* Pat O'Sullivan (IBM)

## Minutes:
* Michal presented a new updated [diagram](../documents/igc-rdf_owl-egeria-DIAGRAM-2020-04-02.png) of the mapping between RDF model elements to IGC and Egeria objects.
    * Michal talked through the mappings
    * We have discussed various approaches around how to capture the model, the main aspects are :
        * Glossary with Taxonomy classification will be represented as an owl:ontology
        * Glossary Category will be represented as a rdfs:container 
        * Glossary Term with SpineObject classification will be represented as an rdfs:class
        * Glossary Term with Spine Attribute will be represented by rdf:property
        * There is a specially name Glossary Category for subject are classification.
        * Glossaries, Terms, Categories all can take name, description which are rdfs:label and rdf:comment  
        * Glossary Term examples will come from rdfs:examples
        * TermAnchor, CategoryAnchor will be mapped from the rdfs:member
        * Has-a relationship is represented be the range and domains between a rdfs:class and rdfs:property
        * validValue relationship and glossaryTerm data value classification is when there is only a rdf:property -> rdfs:domain -> rdfs:class. We  
        * is-a-type-of relationship is a rdfs:subClassOf (question should this be isa ?)
        * Synonym relationship is rdfs:sameAs 
        * related term is any other domain and range between rdfs:class to rdfs:class or rdfs:property to rdfs:property  
   * the only non-standard representation in the model is how we identify subject areas.      
   * Talked of licenses following the semantic content
   * Talked of needing a willing partner to checkout how this sort of model content could be consumed into other non-IBM tools.
   * Talked of potentially adding new Egeria capabilities to be able to represent some of the IGC labels. 
                     
## Actions:
* David and michal to continue to test the proposal with the view to creating a prototype Egeria parser.
* Mandy to fix the CIM parser.
* Pat to talk with OMs so confirm this approach 
* David to confirm that Michals industry model CIM models still parse into Egeria  
* Graham to prototype CIM model with the Egeria visualisation REX.

 
## Next session:
* TBA 