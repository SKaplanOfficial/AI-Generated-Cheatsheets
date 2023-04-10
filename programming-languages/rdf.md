# RDF Cheatsheet

## Unique Features
- Data model for representing information in a machine-readable format
- Based on subject-predicate-object triples
- Supports linking data across different sources and domains
- Widely used in the semantic web and linked data applications
- Can be queried using SPARQL

## Triples
```rdf
subject predicate object
```

## Namespaces
```rdf
@prefix prefix_name: <namespace_URI> .
```

## Blank Nodes
```rdf
_:blank_node_name
```

## Literals
```rdf
"literal_value"
"literal_value"^^<datatype_URI>
```

## RDF Collections
```rdf
( item1 item2 item3 )
```

## RDF Lists
```rdf
rdf:List rdf:first item1 ; rdf:rest rdf:nil .
rdf:List rdf:first item1 ; rdf:rest [ rdf:first item2 ; rdf:rest rdf:nil ] .
```

## RDF Schema
```rdf
rdfs:Class
rdfs:subClassOf
rdfs:subPropertyOf
rdfs:domain
rdfs:range
```

## Ontologies
```rdf
owl:Ontology
owl:imports
owl:Class
owl:ObjectProperty
owl:DatatypeProperty
owl:inverseOf
owl:TransitiveProperty
```

## Resources
- [RDF 1.1 Primer](https://www.w3.org/TR/rdf11-primer/)
- [RDFLib](https://rdflib.readthedocs.io/) (Python library for working with RDF)
- [Apache Jena](https://jena.apache.org/) (Java framework for working with RDF and SPARQL)
- [TopBraid Composer](https://www.topquadrant.com/products/topbraid-composer/) (ontology editor and development environment)