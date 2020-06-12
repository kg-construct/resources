# Mapping Languages for Knowledge Graph Construction

## Mapping Language X:
- **Name**:
- **specification**: 
- **year**:
- **syntax(RDF or not RDF, if not RDF, what?)**:
- **description**: 
- **data source limitations (If yes, what limitations? By default, we assume languages generating RDF can support any data format)**:
- **features (select from the list)**: 
  - collections/lists → can collections/lists be generated with this language?
  - named graphs → are named graphs supported?
  - blank nodes → can blank nodes be generated?
  - data transformations/functions → can data transformations be handled?
  - joining data sources → can the language support joins? If so, on which basis?
    - By ID (e.g., how you typically join database tables)
    - By structure (e.g., a JSON object’s children should be mapped as objects of a relation)
    - other (add any other type of join supported and we haven’t thought of)
  - RDF* support
  - add your own
- **website**:
- **test-cases**: 
- **contact point**: 


## Mapping Language 1:
- **Name**: RML
- **specification**: https://rml.io/specs/rml/
- **year**: 2013
- **syntax**: RDF
- **description**: RML is a generation of the W3C recommended R2RML aiming to support heterogeneous data
- **data source limitations**: no
- **features**: named graphs, blank nodes, data transformations with FnO extension, joins
- **website**: RML.io
- **test-cases**: https://rml.io/test-cases/
- **contact point**: Anastasia Dimou
