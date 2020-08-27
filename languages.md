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

## Mapping Language 2:
- **Name**: SPARQL-Generate
- **specification**: see [_Maxime Lefrançois, Antoine Zimmermann, Noorani Bakerally A SPARQL extension for generating RDF from heterogeneous formats, In Proc. Extended Semantic Web Conference, ESWC, May 2017, Portoroz, Slovenia_](http://www.maxime-lefrancois.info/docs/LefrancoisZimmermannBakerally-ESWC2017-Generate.pdf) for the specification of the first version.
- **year**: 2016
- **syntax**: See [Javacc](https://github.com/sparql-generate/sparql-generate/blob/master/sparql-generate-jena/src/main/javacc/spargl.jj), [extension of YASQE](https://github.com/sparql-generate/sparql-generate-editor/blob/gh-pages/lib/grammar/sparql11-grammar.pl), extension of [Sublime Linked Data package](https://github.com/sparql-generate/sublime-editor/blob/master/src/syntax/sparql-generate.sublime-syntax-source)
- **description**: SPARQL-Generate is an expressive template-based language to generate RDF streams or text streams from RDF datasets and document streams in arbitrary formats
- **data source limitations**: no
- **features**: 
    - collections/lists [(try out)](https://ci.mines-stetienne.fr/sparql-generate/playground.html#ex=example/generate/08-Lists),
    - querying named graphs: yes as it's an extension of SPARQL
    - blank nodes: yes as it's an extension of SPARQL
    - data transformations/function (the standard SPARQL ones, plus the [SPARQL Function form O. Corby and C. Faron Zucker](http://ns.inria.fr/sparql-extension/#function) ) 
    - joining data sources: 
        - By ID, potentially with any data transformation
        - By structure (e.g., a JSON object’s children are mapped as objects of a relation, or even subjects or predicates of relations)
        - [try out the example of a query that combines JSON weather station reports with lists of events described in XML documents and obtained from an external web service](https://ci.mines-stetienne.fr/sparql-generate/playground.html#ex=example/generate/06-DifferentSources)
    - generating RDF streams
    - generating output as HDT
    - IRIs or Literals can be generated with bits of different data sources
    - binary data
- **website**: 
    - https://ci.mines-stetienne.fr/sparql-generate/
- **test-cases**: https://ci.mines-stetienne.fr/sparql-generate/playground.html
- **contact point**: Maxime Lefrançois, EMSE Saint-Étienne

## Mapping Language 3:
- **Name**: ShExML
- **specification**: http://shexml.herminiogarcia.com/spec/ 
- **year**: 2019
- **syntax**: Based on ShEx syntax but with its own grammar ([ANTLR4 grammar](https://github.com/herminiogg/ShExML/blob/master/src/main/java/es/weso/antlr/ShExMLParser.g4))
- **description**: ShExML is a language based on ShEx to map and merge heterogeneous data sources. It is designed with usability in mind trying to make the script creation easier to the users.
- **data source limitations**: no
- **features (select from the list)**: 
  - collections/lists → no
  - named graphs → no (future extension)
  - blank nodes → yes
  - data transformations/functions → limited ones (see [String operators](http://shexml.herminiogarcia.com/spec/#string-operation-over-iterators) and [Matchers](http://shexml.herminiogarcia.com/spec/#string-operation-over-iterators)), planning to add an extensible function library
  - joining data sources:
    - By ID: [JOIN keyword](http://shexml.herminiogarcia.com/spec/#join-over-iterators)
    - By structure: [Shape linking](http://shexml.herminiogarcia.com/spec/#linking-shapes)
- **website**: http://shexml.herminiogarcia.com/
- **test-cases**: https://github.com/herminiogg/ShExML/tree/master/src/test/scala-2.12/es/weso/shexml
- **contact point**: Herminio García González (garciaherminio@uniovi.es)
