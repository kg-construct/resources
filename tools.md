# Knwoledge Graph Construction Tools
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
