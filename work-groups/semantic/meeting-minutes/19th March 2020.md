# Egeria Semantics workgroup 19th of March

## Agenda:
* Michal to present assessment of model formats and mappings from RDF to Egeria to IGC  

## Attendees:
* David Radley (IBM)
* Mandy Chessell (IBM)
* Michal Miklas (IBM)
* Stefhan Van Hevoirt (ING)
* Oana Turbatu (ING)
* Pat O'Sullivan (IBM)

## Minutes:
* Michal presented his investigations around mappings of RDF model elements to IGC and Egeria objects.
 [spreadsheet](../documents/19th%20March%20Egeria-rdf-mappings.xlsx)
    * Michal talked of the many standards around model element standards. He was particularly interested in how to represent a containment relationship.
    * Michal was keen to copy the gs1 style of elements, whereby elements could be associated with annotations from different namesapces, for example the rdfs and the 
    owl class annotations would both be applied to an element, so that consumers that did not understand owl could pick up the rdfs tag         
    * We talked of how Egeria's Subject Area can be represented in IGC.
        * As a label - Michal and Pat felt this was a natural fit. 
        * As a term - a 'classification' term could be associated with the real term
        * As a category - where all the terms in a category would b in a subject area.
    * we talked about the difference between a spine object and attribute and a subject area in 2 ways
        * Subject Area classifications could be specified on a set of standard definitions. for example models supplied by a vendor that could 
        be used asis. This approach would be to "use the standard definitions" 
        * Subject Area can be also thought of as representative of the structure of an orgnisation. So sets of experts in the organisation naturally
        form subject areas and groups of associated metadata. This approach would be when the standard model does not fit the organisation structure and 
        so the standard model cannot be used.        
    * We talked of identifying elements from their relationships. 
    * We talked of the ideal way of representing model content using RDFS etc tags - so that it is self descriptive and would 'naturally' map into 
     Egeria (IBM products would also be able to consume this form directly); using open standards where possible to make the format as widely consumable as possible.
    * We talked of 2 ways to recognise an Egeria glossary, when importing from a metadata repository that only has categories (such as IGC)
    We could import all content into one Egeria glossary or alternatively we could import all Categories that do not have parents as glossaries.
    If there is an explicit canonical vocabulary, then this would be identified as a Canonical Glossary                 
## Actions:
* David to circulate the mappings and the proposals for feedback.
 
## Next session:
* consolidate any feedback, Michal to present his progress on creating an RDF generator and agree next steps.