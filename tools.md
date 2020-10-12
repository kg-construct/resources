# Knowledge Graph Construction Tools
Description of the tools for knowledge graph construction

## Tool X (TEMPLATE):
- **Name of the tool**:
- **Description**:
- **Repository (link to the tool’s repository)**:
- **Website (if is different to the repository)**:
- **Open source? (If not open sourced, ideally provide an option to test it)**:
- **Year introduced**:
- **Contact person (who is the main contact person?)**:
- **Purpose (what can one do with the tool?)**: Select one of this options: Processor (executes rules to generate a knowledge graph), editor (automatically o manually generation of mapping rules), other (e.g., pre-processing)
- **Mapping language**: (which mapping language(s) is supported by the tool)
- **Supported data (formats, sizes)**:
- **Programming language**:
- **Special features**:
- **DOI**:
- **License**:
- **Test cases**: (if any for the supported languages)
- **Related use cases**: (specify use cases shared with the community group (if any) where the tool is used)
- **Related projects**: (specify projects (if any) where the tool is used, ideally provide links to the projects descriptions)


## Tool 1:
- **Name of the tool**: Morph-CSV
- **Description**: Morph-CSV is an open source tool for querying tabular data sources using SPARQL. It exploits the information from the query, RML+FnO mappings and CSVW metadata to enhance the performance and completness of traditional OBDA systems (SPARQL-to-SQL translators). At this moment can be embebed in the top of any R2RML-compliant system.
- **Repository**: https://github.com/oeg-upm/morph-csv
- **Website**: https://morph.oeg.fi.upm.es/tool/morph-csv
- **Open source**: Yes
- **Year introduced**: 2019
- **Contact person**: David Chaves (dchaves@fi.upm.es)
- **Purpose**: Other (Enhance SPARQL-to-SQL engines when data is in CSV)
- **Mapping language**: YARRRML+FnO and CSVW
- **Supported data**: CSV (tested with BSBM 360K products)
- **Programming language**: Python + Bash
- **DOI**: https://doi.org/10.5281/zenodo.3731941
- **License**: Apache-2.0
- **Related use cases**: https://github.com/kg-construct/use-cases/blob/master/oeg-publictransport.md
- **Related projects**: http://sprint-transport.eu/

## Tool 2:
- **Name of the tool**: RMLEditor
- **Description**: The RMLEditor offers a graphical user interface to create rules to generate knowledge graphs based on heterogeneous data sources.
- **Repository (link to the tool’s repository)**: https://github.com/RMLio/rmleditor-ce
- **Website (if is different to the repository)**: https://app.rml.io/rmleditor/
- **Open source? (If not open sourced, ideally provide an option to test it)**: No
- **Year introduced**: 2016
- **Contact person (who is the main contact person?)**: Pieter Heyvaert (pieter.heyvaert@ugent.be)
- **Purpose (what can one do with the tool?)**: editor
- **Mapping language**: [R2]RML
- **Supported data (formats, sizes)**: CSV, JSON, XML
- **Programming language**: HTML/CSS/JS
- **Special features**: Uses LOV to find relevant classes and properties. Uses MapVOWL to visualize rules.
- **DOI**: N/A
- **License**: Free community edition with limitations and paid edition without limitations. 
- **Test cases**: None
- **Related use cases**: None
- **Related projects**: [DyVerSIFy](https://www.imec-int.com/en/what-we-offer/research-portfolio/dyversify), [MOS2S](https://www.mos2s.eu/), [COMBUST](https://www.imec-int.com/en/what-we-offer/research-portfolio/combust)

## Tool 3:
- **Name of the tool**: RMLMapper
- **Description**: The RMLMapper executes RML rules to generate high quality Linked Data from multiple originally (semi-)structured data sources
- **Repository (link to the tool’s repository)**: https://github.com/RMLio/rmlmapper-java
- **Website (if is different to the repository)**; https://rml.io
- **Open source? (If not open sourced, ideally provide an option to test it)**: Yes
- **Year introduced**: 2014
- **Contact person (who is the main contact person?)**: Ben De Meester (ben.demeester@ugent.be)
- **Purpose (what can one do with the tool?)**: Processor
- **Mapping language**: RML, R2RML
- **Supported data (formats, sizes)**: local and remote files (CSV using ql:CSV or CSVW, JSON using JSONPath, XML using XPath), databases (MySQL, PostgreSQL, SQLServer, OracleDB). The mapper is in-memory, so query result size should be less than the machine's memory
- **Programming language**: JAVA
- **Special features**: Extensible in terms of supported data formats, Configurable and extensible data transformations using https://FnO.io, interdatasource join. Reference implementation of RML.
- **DOI**: N/A
- **License**: MIT
- **Test cases**: https://rml.io/test-cases/
- **Related use cases**: betweenourworlds-anime, idlab-covid19, idlab-dbpedia, idlab-facebook, idlab-twitter, idlab-velopark
- **Related projects**: [EcoDaLo], [ESSENCE], [DAIQUIRI], [DiSSeCt]

[EcoDaLo]: https://www.imec-int.com/en/what-we-offer/research-portfolio/ecodalo
[ESSENCE]: https://www.imec-int.com/en/what-we-offer/research-portfolio/essence
[DAIQUIRI]: https://www.imec-int.com/en/what-we-offer/research-portfolio/daiquiri
[DiSSeCt]: https://dissectsite.wordpress.com/

## Tool 4:
- **Name of the tool**: Morph-RDB
- **Description**: Morph-RDB (formerly called ODEMapster) is an RDB2RDF engine developed by the Ontology Engineering Group, that follows the R2RML specification (http://www.w3.org/TR/r2rml/).This engine supports two operational modes: data upgrade (generating RDF instances from data in a relational database) and query translation (SPARQL to SQL). Morph-RDB employs various optimisation techniques in order to generate efficient SQL queries, such as self-join elimination and subquery elimination. 
- **Repository**: https://github.com/oeg-upm/morph-rdb
- **Website**: https://morph.oeg.fi.upm.es/tool/morph-rdb
- **Open source**: Yes
- **Year introduced**: 2014
- **Contact person**: David Chaves (dchaves@fi.upm.es)
- **Purpose**: Processor
- **Mapping language**: R2RML
- **Supported data**: SQL (tested with MySQL and PostgreSQL)
- **Programming language**: Scala + Java
- **DOI**: N/A
- **License**: Apache-2.0
- **Related use cases**: https://github.com/kg-construct/use-cases/blob/master/oeg-publictransport.md
- **Related projects**: http://sprint-transport.eu/, https://www.mobile-age.eu/, https://bimerr.eu/

## Tool 5:
- **Name of the tool**: Morph-GraphQL
- **Description**: Morph-GraphQL is an open source system for generating GraphQL servers automatically from declarative mappings such as R2RML or RML. Currently, Morph-GraphQL is able to generate GraphQL servers in JavaScript and SQL databases. Current experimental features include the generation of GraphQL server in other languages (e.g. Java) and other data models (e.g. MongoDB)
- **Repository**: https://github.com/oeg-upm/morph-graphql
- **Website**: https://morph.oeg.fi.upm.es/tool/morph-graphql
- **Open source**: Yes
- **Year introduced**: 2019
- **Contact person**: David Chaves (dchaves@fi.upm.es)
- **Purpose**: Processor
- **Mapping language**: R2RML and RML
- **Supported data**: SQL (tested with H2) and NoSQL (experimental, tested with MongoDB)
- **Programming language**: JavaScript/Node.js
- **DOI**: N/A
- **License**: Apache-2.0
- **Related use cases**: N/A
- **Related projects**: N/A

## Tool 6:
- **Name of the tool**: Mapeathor
- **Description**: Mapeathor is a simple spreadsheet parser able to generate mapping rules in three mapping languages: R2RML, RML (with extension to functions from FnO) and YARRRML. It takes the mapping rules expressed in a spreadsheet (designed to facilitate the mapping rule writting process) and transforms them into the desired language. 
- **Repository (link to the tool’s repository)**: https://github.com/oeg-upm/Mapeathor
- **Website (if is different to the repository)**: https://morph.oeg.fi.upm.es/tool/mapeathor
- **Open source? (If not open sourced, ideally provide an option to test it)**: Yes
- **Year introduced**: 2019
- **Contact person (who is the main contact person?)**: Ana Iglesias (ana.iglesiasm@upm.es)
- **Purpose (what can one do with the tool?)**: Editor
- **Mapping language**: R2RML, RML, YARRRML
- **Supported data (formats, sizes)**: Excel
- **Programming language**: Python
- **License**: Apache-2.0
- **Test cases**: None
- **Related use cases**: None
- **Related projects**: [Ciudades Abiertas](http://www.ciudadesabiertas.es/)

## Tool 7:
- **Name of the tool**: SDM-RDFizer
- **Description**: SDM-RDFizer is an interpreter of mapping rules that allows the transformation of (un)structured data into RDF knowledge graphs.
- **Repository (link to the tool’s repository)**: https://github.com/SDM-TIB/SDM-RDFizer
- **Open source? (If not open sourced, ideally provide an option to test it)**: Yes
- **Year introduced**: 2017
- **Contact person (who is the main contact person?)**: Enrique Iglesias (s6enigle@uni-bonn.de)
- **Purpose (what can one do with the tool?)**:  Transformation of (un)structured data into RDF knowledge graphs by an efficient execution of RML triple maps.
- **Mapping language**: RML (current version)
- **Supported data (formats, sizes)**: CSV, JSON, RDB, XML
- **Programming language**: Python
- **Special features**: The SDM-RDFizer implements optimized data structures and relational algebra operators that enable an efficient execution of RML triple maps even in the presence of Big data. SDM-RDFizer is also extensible in terms of supported data formats, Configurable and extensible data processing functions using https://FnO.io
- **DOI**: https://doi.org/10.5281/zenodo.3872103
- **License**: Apache-2.0
- **Test cases**: https://rml.io/test-cases/
- **Related use cases**: https://github.com/kg-construct/use-cases/blob/master/sdm-genomics.md
- **Related projects**: [iASiS](http://project-iasis.eu/), [BigMedilytics - lung cancer pilot](https://www.bigmedilytics.eu/), [CLARIFY](https://www.clarify2020.eu/), [P4-LUCAT](https://www.tib.eu/de/forschung-entwicklung/projektuebersicht/projektsteckbrief/p4-lucat), [ImProVIT](https://www.tib.eu/de/forschung-entwicklung/projektuebersicht/projektsteckbrief/improvit), [PLATOON](https://platoon-project.eu/)

## Tool 8:
- **Name of the tool**: RMLStreamer
- **Description**: The RMLStreamer executes RML rules to generate high quality Linked Data from multiple originally (semi-)structured data sources in a streaming way. 
- **Repository (link to the tool’s repository)**: https://github.com/RMLio/RMLStreamer
- **Website (if is different to the repository)**: https://rml.io
- **Open source? (If not open sourced, ideally provide an option to test it)**: Yes
- **Year introduced**: 2019
- **Contact person (who is the main contact person?)**: Gerald Haesendonck (gerald.haesendonck@ugent.be)
- **Purpose (what can one do with the tool?)**: Processor
- **Mapping language**: RML
- **Supported data (formats, sizes)**: formats: CSV, XML, JSON; media: files, TCP sockets, Kafka topics
- **Programming language**: Scala
- **Special features**: Extensible in terms of supported data formats and media, optimised for processing big data sets and contious data streams, designed to run on a cluster.
- **DOI**: https://doi.org/10.5281/zenodo.3887065
- **License**: MIT
- **Test cases**: https://rml.io/test-cases/
- **Related use cases**: https://github.com/kg-construct/use-cases/blob/master/idlab-twitter.md
- **Related projects**: [MOS2S], [DyVerSIFy], [ESSENCE], [DAIQUIRI]

[MOS2S]: https://www.mos2s.eu/
[DyVerSIFy]: https://www.imec-int.com/en/what-we-offer/research-portfolio/dyversify


## Tool 9:
- **Name of the tool**: SPARQL micro-services
- **Description**:
    The SPARQL Micro-Service architecture is meant to unlock data silos hidden behind proprietary Web APIs by equipping them with a lightweight SPARQL endpoint. The whole idea is about bringing Web APIs into the Web of Data and making it possible to integrate Linked Data and Web APIs within a simple federated SPARQL query. 
    
    A SPARQL micro-service encapsulates a Web API and typically yields a **small, resource-centric graph** generated dynamically. It can be seen as a **configurable** SPARQL endpoint in that it expects parameters, e.g. a SPARQL micro-service to find photos from Snapshat may expect tags.
    
    An interesting use of SPARQL micro-services is to **assign dereferenceable URIs to Web API resources** that do not have URIs in the first place. For instance, https://sparql-micro-services.org/ld/flickr/photo/31173091626 is the dereferenceable URI of a photo in Flickr. The content is generated dynamically based on the photo identifier.
- **Repository (link to the tool’s repository)**: https://github.com/frmichel/sparql-micro-service
- **Website (if is different to the repository)**: example SPARQL micro-services: https://sparql-micro-services.org/
- **Open source? (If not open sourced, ideally provide an option to test it)**: yes
- **Year introduced**: 2018
- **Contact person (who is the main contact person?)**: Franck Michel (franck.michel@cnrs.fr)
- **Purpose (what can one do with the tool?)**: processor, other
- **Mapping language**: (which mapping language(s) is supported by the tool) : SPARQL construct
- **Supported data (formats, sizes)**: mainly JSON-based Web APIs, XML-based Web APIs can be adapted too
- **Programming language**: php 
- **Special features**:
    - Docker deployment ready
    - Assign dereferenceable URIs to Web API resources (bridge Web APIs and LOD)
    - Provide provenance information as part of the graph generated
    - Simple configuration with a config.ini file, or with rich SPARQL Sescription Description and SHACL shapes graph
    - Dynamic generation of HTML documentation + test interface from the SPARQL micro-service Sescription Description see [example](https://sparql-micro-services.org/service/flickr/getPhotosByTags_sd/))
    - Autmatic markup of HTML documentation as schema.org Dataset to allow webscale discoverability of SPARQL micro-services, e.g. with Google Dataset Search
- **DOI**: n/a
- **License**: Apache 2.0
- **Test cases**: n/a
- **Related use cases**: https://github.com/kg-construct/use-cases/blob/master/inria-kg-vs-webapis.md
- **Related projects**: [Taxref-Web](https://taxref.mnhn.fr/taxref-web/) (private access only, comparison of 20+ Web APIs in the biodiversity domain). Multiple hands-on sessions experimented successfully with various Web APIs: Flickr, Youtube, Twitter, Spotify, Deezer, Musicbrainz...

## Tool 10:
- **Name of the tool**: WordLift Plugin
- **Description**: 

WordLift is a WordPress plugin that brings state-of-the-art semantic technologies to the hands of any blogger and publisher: without requiring any technical skills, it helps produce richer content and organize it by suggesting facts and information to provide readers with meaningful context and adding semantic markup to the text to help machines fully understand any website.

Features:

  * Text Analysis: WordLift analyzes content and identifies matching entities organized in 4 categories: Who, What, When and Where.
  * Tag Content: Editors can accept the suggested entities to add contextual info for the user, efficiently selecting internal links to existing content.
  * Create New Entities: Editors can create new entities providing additional context and enriching the web site Knowledge Graph. WordLift will learn and next time they will be detected.
  * Edit Entities: Editors can edit all entities to customize the Knowledge Graph around the web sites' audiences and build new relationships.
  * Images: WordLift suggests open license images and media from own library, saving the time usually spent searching for visuals.
  * Geomaps: Locations in articles can quickly be mapped adding the Geomap widget.
  * Timelines: Events can be displayed chronologically adding the Timeline widget.
  * Chords: Visualize what relates to what in every article adding the Chord widget.
  * Navigator: Recommend relevant articles adding the Navigator widget.
  * Faceted Search: Suggest additional content related to the topics found in your article, letting readers dive into your archive with the Faceted Search widget.
  * Meaningful Navigation: WordLift automatically identifies topics in articles, using Wikipedia’s classification system. This allows to create new entry points for content based on topics, events, people and places.
  * Publish Search Data: WordLift automatically adds schema.org markup articles, allowing search engines to properly index and display content and intelligent agents such as Siri and Alexa to access it.
  * Publish Linked Data: WordLift publishes content’s metadata.

- **Repository**: https://github.com/insideout10/wordlift-plugin
- **Website**: https://wordlift.io
- **Open source?**: yes
- **Year introduced**: 2017
- **Contact person**: David Riccitelli (david@wordlift.io)
- **Purpose**: editor, other
- **Mapping language**: n/a
- **Supported data**: WordPress, unstructured HTML
- **Programming language**: PHP, Java, Python
- **Special features**: [Knowledge Graph](https://wordlift.io/blog/en/entity/knowledge-graph/), [Linked Data](https://wordlift.io/blog/en/entity/linked-data/), NLP, SPARQL, GraphQL, Persistent URIs
- **DOI**: n/a
- **License**: GPL
- **Test cases**: n/a
- **Related use cases**: https://github.com/kg-construct/use-cases/blob/master/wordlift-salzburgerland.md
- **Related projects**: [WordLift NG]

[WordLift NG]: https://wordlift.io/blog/en/wordlift-next-generation-receives-grant-from-eu/


## Tool 11:
- **Name of the tool**: RocketRML
- **Description**: An efficient RML-mapper implementation with Javascript for the RDF mapping language (RML).
- **Repository (link to the tool’s repository)**: https://github.com/semantifyit/RocketRML
- **Website (if is different to the repository)**: https://semantifyit.github.io/RocketRML/
- **Open source? (If not open sourced, ideally provide an option to test it)**: Yes
- **Year introduced**: 2019
- **Contact person (who is the main contact person?)**: Umutcan Simsek (umutcan.simsek@sti2.at)
- **Purpose (what can one do with the tool?)**: Processor
- **Mapping language**: RML (in Turtle and YARRML syntax)
- **Supported data (formats, sizes)**: CSV, JSON, XML. Tested with 500k triples (takes ~20s)
- **Programming language**: Javascript (Node.js)
- **Special features**: It efficiently maps hierarchical sources by using some caching mechanisms for iterators and JOIN results. Available as a tool with CLI and as an NPM package. A Dockerfile is also provided. Please see the Github repository.
- **DOI**: n/a
- **License**: CC-BY-SA-4.0
- **Test cases**: n/a
- **Related use cases**: TBD
- **Related projects**: [semantify.it], [MindLab]

[semantify.it]: https://semantify.it
[MindLab]: https://mindlab.ai


## Tool 12:
- **Name of the tool**: SPARQL-Generate
- **Description**: SPARQL-Generate is an expressive template-based language to generate RDF streams or text streams from RDF datasets and document streams in arbitrary formats
- **Repository (link to the tool’s repository)**: https://github.com/sparql-generate/sparql-generate
- **Website (if is different to the repository)**: https://ci.mines-stetienne.fr/sparql-generate/
- **Open source? (If not open sourced, ideally provide an option to test it)**: yes
- **Year introduced**: 2016
- **Contact person (who is the main contact person?)**: Maxime Lefrançois, MINES Saint-Étienne
- **Purpose (what can one do with the tool?)**: Processor
- **Mapping language**: SPARQL-Generate
- **Supported data (formats, sizes)**: RDF, SQL, XML, JSON, CSV, GeoJSON, HTML, CBOR, plain text with regular expressions, large CSV documents (unofficially: generation of 17.5 M triples HDT in < 9'20''), MQTT or WebSocket streams, repeated HTTP GET operations. 
- **Programming language**: Java
- **Special features**: 
    - useable [on the web playground](https://ci.mines-stetienne.fr/sparql-generate/playground.html), [inside Sublime Text](https://ci.mines-stetienne.fr/sparql-generate/sublime.html), [as an executable JAR](https://ci.mines-stetienne.fr/sparql-generate/language-cli.html), [as an open source Java library](https://ci.mines-stetienne.fr/sparql-generate/get-started.html) ;
    - can also generate text streams from RDF datasets and document streams in arbitrary format (implements something like [STTL](https://ns.inria.fr/sparql-template/)).
- **DOI**: https://doi.org/10.5281/zenodo.3965916
- **License**: Apache 2
- **Test cases**: see https://ci.mines-stetienne.fr/sparql-generate/playground.html 
- **Related projects**: [ITEA2 12004 SEAS (Smart Energy Aware Systems)], [ANR 14-CE24-0029 OpenSensingCity], [ETSI STF 578], bilateral research contracts with ENGIE R&D CRIGEN, [ANR 19-CE23-0012 CoSWoT], [ANR HyperAgents].

[ITEA2 12004 SEAS (Smart Energy Aware Systems)]: https://itea3.org/project/seas.html
[ANR 14-CE24-0029 OpenSensingCity]: https://anr.fr/Project-ANR-14-CE24-0029
[ETSI STF 578]: https://portal.etsi.org/STF/STFs/STF-HomePages/STF578 
[ANR 19-CE23-0012 CoSWoT]: https://anr.fr/Project-ANR-19-CE23-0012
[ANR HyperAgents]: http://hyperagents.gitlab.emse.fr/

## Tool 13:
- **Name of the tool**: ShExML
- **Description**: ShExML engine and webapp
- **Repository**: https://github.com/herminiogg/ShExML
- **Website (if is different to the repository)**: http://shexml.herminiogarcia.com
- **Open source?**: yes
- **Year introduced**: 2019
- **Contact person**: Herminio García González (garciaherminio@uniovi.es)
- **Purpose**: Processor (executes rules to generate a knowledge graph), editor (automatically o manually generation of mapping rules), translator (convert ShExML rules to RML rules)
- **Mapping language**: ShExML
- **Supported data**: XML, JSON, CSV.
- **Programming language**: Scala
- **Special features**: N/A
- **DOI**: N/A
- **License**: Not yet decided
- **Test cases**: https://github.com/herminiogg/ShExML/tree/master/src/test/scala-2.12/es/weso/shexml (sbt test and [CI](https://travis-ci.org/github/herminiogg/ShExML))
- **Related use cases**: [Asturian Notaries Manuscripts](https://github.com/kg-construct/use-cases/blob/master/uniovi-notaries.md)
- **Related projects**: N/A

## Tool 14:
- **Name of the tool**: CARML
- **Description**: An extensible RML mapping engine with built-in support for JSON, CSV, and XML
- **Repository (link to the tool’s repository)**: https://github.com/carml/carml
- **Website (if is different to the repository)**:
- **Open source? (If not open sourced, ideally provide an option to test it)**: Yes
- **Year introduced**: 2017
- **Contact person (who is the main contact person?)**: Pano Maria (pano@skemu.com)
- **Purpose (what can one do with the tool?)**: Processor
- **Mapping language**: RML
- **Supported data (formats, sizes)**: CSV, JSON, XML
- **Programming language**: JAVA
- **Special features**: Easily extensible for other formats. InputStream extension for easy programmatic binding of sources. XML document extension to be able to use namespace prefix mappings in XPath expressions. Support for FnO functions. 
- **DOI**: n/a
- **License**: MIT
- **Test cases**: https://rml.io/test-cases/
- **Related use cases**: [Kadaster Data Platform](https://github.com/kg-construct/use-cases/blob/master/kadaster-ld.md)
- **Related projects**: [Kadaster Data Platform (PDOK)](https://www.pdok.nl/), [Zazuko XRM](https://zazuko.com/products/expressive-rdf-mapper/), [DotWebStack Framework](https://github.com/dotwebstack/dotwebstack-framework/)

## Tool 15:
- **Name of the tool**: Helio
- **Description**: Helio is a framework that allows publishing RDF data from different heterogeneous sources as Linked Data
- **Repository (link to the tool’s repository)**: https://github.com/oeg-upm/Helio
- **Website (if is different to the repository)**: https://oeg-upm.github.io/Helio/
- **Open source? (If not open sourced, ideally provide an option to test it)**: Yes
- **Year introduced**: 2018
- **Contact person (who is the main contact person?)**: Andrea Cimmino (cimmino@fi.upm.es)
- **Purpose (what can one do with the tool?)**: Processor (executes rules to generate a knowledge graph),  Publish Knowledge Graph.
- **Mapping language**: RML, WoT-Mapping, and Helio mapping
- **Supported data (formats, sizes)**: CSV, XML, HTML, text, JSON, RDF
- **Programming language**: Java
- **Special features**: relies on a plugin sistem that does not require developers to download the core code, customizable html views, can integrate existing tools that generate RDF.
- **DOI**:
- **License**: APACHE 2.0
- **Test cases**: (if any for the supported languages)
- **Related use cases**: -
- **Related projects**: [VICINITY H2020](https://www.vicinity2020.eu/vicinity/), [DELTA H2020](https://www.delta-h2020.eu/), [BIMER H2020](https://bimerr.eu/about/)

## Tool 16:
- **Name of the tool**: FunMap
- **Description**: FunMap is an interpreter of RML+FnO that converts a data integration system defined using RML+FnO into an equivalent data integration system where RML mappings are function-free.
- **Repository (link to the tool’s repository)**: https://github.com/SDM-TIB/FunMap
- **Open source? (If not open sourced, ideally provide an option to test it)**: Yes
- **Year introduced**: 2020
- **Contact person (who is the main contact person?)**: Samaneh Jozashoori (samaneh.jozashoori@tib.eu)
- **Purpose (what can one do with the tool?)**:  It can be applied when pre-processing step is provided in the context of mapping rules as functions; i.e. the data pre-processing is supposed to be performed at the time of data model transformation (into RDF) and knowledge graph creation.
- **Mapping language**: RML (current version)
- **Supported data (formats, sizes)**: CSV, RDB
- **Programming language**: Python
- **Special features**: FunMap empowers the knowledge graph creation process with optimization techniques to reduce execution time.
- **DOI**: https://doi.org/10.5281/zenodo.3993657
- **License**: Apache-2.0
- **Test cases**: - 
- **Related use cases**: -
- **Related projects**: [CLARIFY](https://www.clarify2020.eu/), [P4-LUCAT](https://www.tib.eu/de/forschung-entwicklung/projektuebersicht/projektsteckbrief/p4-lucat), [Ciudades Abiertas](https://ciudades-abiertas.es/)

## Tool 17:
- **Name of the tool**: Squerall
- **Description**: An implementation of the so-called _Semantic Data Lake_, a query engine _uniformly_ accessing original large and heterogeneous data sources using Semantic Web principles and technologies
- **Repository (link to the tool’s repository)**: https://github.com/EIS-Bonn/Squerall
- **Website (if is different to the repository)**: https://eis-bonn.github.io/Squerall/
- **Open source? (If not open sourced, ideally provide an option to test it)**: Yes
- **Year introduced**: 2017.
- **Contact person (who is the main contact person?)**: Mohamed Nadjib Mami (mohamed.nadjib.mami@gmail.com)
- **Purpose (what can one do with the tool?)**: Processor (executes rules to generate a knowledge graph). Squerall is a virtual OBDA (Ontology Based Data Access) engine, where a knowledge graph is only constirbuted _on-the-fly_ at query-time. However, with a slight development effort, it would be possible to physically materialize the knowledge graph (in RDF) following a property table partitining-like scheme.
- **Mapping language**: RML
- **Supported data (formats, sizes)**: CSV, Parquet, MongoDB, Cassandra, JDBC (MySQL, SQL Server, etc.), (beta) Elasticsearch. Squerall can be [extended](https://github.com/EIS-Bonn/Squerall#extensibility) to support other sources
- **Programming language**: Scala, Java
- **Special features**: Use SPARQL to query popular distributed data sources, e.g. files in Hadoop, NoSQL stores _on-the-fly_ i.e. without requiring pre-processing or ingestion. Disparate data may be joinable by declaratively altering some of its atrributes thanks to the use of the FnO ontology. State-of-the-art Big Data query engines are used for the querying, namely Apache Spark and Presto. Squerall can programmatically be [extended](https://github.com/EIS-Bonn/Squerall#extensibility) to use another query engines e.g. Drill or Dremio)
- **DOI**: https://zenodo.org/record/2636436#.X3tOY_kzZPY
- **License**: Apache-2.0

## Tool 18:
- **Name of the tool**: Chimera
- **Description**: Chimera is a tool to build conversion pipelines leveraging Semantic Web technologies.  It is built on-top of Apache Camel to easily configure message-to-message mediators or batch converters using lifting/lowering procedures to/from a reference ontology. In principle the aim is to completely avoid coding by just configuring a pipeline using the various blocks provided.
- **Repository (link to the tool’s repository)**: [https://github.com/cefriel/chimera](https://github.com/cefriel/chimera)
- **Open source?** : YES
- **Year introduced**: 2019
- **Contact person (who is the main contact person?)**: Mario Scrocca ([mario.scrocca@cefriel.com](mailto:mario.scrocca@cefriel.com))
- **Purpose (what can one do with the tool?)**: A basic Chimera pipeline involves a lifting Processor (fork of the RMLMapper) Tool and a lowering Processor ([rdf-lowerer](https://github.com/cefriel/rdf-lowerer) built on Apache Velocity). Additional blocks, e.g., for pre-processing/enrichment of the knowledge graph, can be integrated in the pipeline.
- **Mapping language**: RML for lifting, _extended_ VTL (Velocity Template Language) for lowering
- **Supported data (formats, sizes)**: CSV, JSON, XML
- **Programming language**: Java
- **Special features**: High configurability of pipelines to satisfy different data integration requirements using Semantic Web Technologies. Easy to integrate with existing data sources and sinks thanks to Apache Camel components.
- **License**: Apache-2.0
- **Related use cases**:https://github.com/kg-construct/use-cases/blob/master/oeg-publictransport.md
- **Related projects**: http://sprint-transport.eu/



## Tool 19:
- **Name of the tool**: Ontario
- **Description**: A federated query processing engine that is able to access heterogeneous data sources in a Semantic Data Lake. Ontario leverages the concept of RDF Molecule Templates to effectively and efficeintly decompose, plan and execute SPARQL queries over a federation of data sources. The given SPARQL queries are transformed to the query languages of data sources in a Semantic Data Lake using the mapping rules expressed uring RML language.  
- **Repository (link to the tool’s repository)**: https://github.com/SDM-TIB/Ontario
- **Website (if is different to the repository)**: https://labs.tib.eu/info/projekt/ontario/
- **Open source? (If not open sourced, ideally provide an option to test it)**: Yes
- **Year introduced**: 2017.
- **Contact person (who is the main contact person?)**: Kemele M. Endris (kemele.endris@gmail.com)
- **Purpose (what can one do with the tool?)**: Processor. Ontario is able to answer SPARQL SELECT queries over heterogeneous data sources; CSV, JSON, XML, RDBMS, Neo4j, MongoDB, RDF. Non-RDF data is transformed on-the-fly during query time. Ontario also support SPARQL CONSTRUCT queries to transform data from a Semantic Data Lake to RDF.
- **Mapping language**: RML
- **Supported data (formats, sizes)**: CSV, Parquet, MongoDB, JDBC (MySQL, Postgres, Neo4j, RDF.
- **Programming language**: Python
- **DOI**: http://doi.org/10.1007/978-3-030-27615-7_29
- **License**: GNU/GPL v2

