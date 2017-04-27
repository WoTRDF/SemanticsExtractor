# SemanticsExtractor
Here we present an example of interoperting three IoT Platforms (i.e., openHAB, EclipseIoT and Datavenue) with Semantics Extractor to automatically generate semantically-rich and interlinked RDF graphs from REST interfaces exposed by IoT platforms. 

Semantics Extractor starts by taking input of three REST entrypoints from three IoT platforms and generate a first with REST Crawler:

![My image](https://github.com/WoTRDF/SemanticsExtractor/blob/master/docs/1.%20REST%20URIs.jpg)

Synxtax Extractor creates a stub RDF graph by extracting syntax information from discvered resources' descriptions:

![My image](https://github.com/WoTRDF/SemanticsExtractor/blob/master/docs/2.%20Syntax%20Extractor%20Output.jpg)


Ontology Matcher identifies RDF graph elements based on semantic keyword matching:

![My image](https://github.com/WoTRDF/SemanticsExtractor/blob/master/docs/3.%20Ontology%20Matching.jpg)


Semantic Reasoner infers the classes and properties in RDF graphs based on ontology property’s domain and range definitions:

![My image](https://github.com/WoTRDF/SemanticsExtractor/blob/master/docs/4.%20Inferring%20of%20Semantic%20Reasoner.jpg)


Semantic Reasoner refines RDF elements following semantic rules, and the refined elements can be further used to deduce other graph elements:

![My image](https://github.com/WoTRDF/SemanticsExtractor/blob/master/docs/5.%20Refining%20of%20Semantic%20Reasoner.jpg)


Link Extractor creates additional implicit links among IoT resources and platforms by capturing data change coincidences. In this example, Classifier further refines the links caputured by Link Extractor based on classification:




At the end,  a RDF graph is generated by Semantics Extractor to interoperate the three IoT platforms via semantics: 





