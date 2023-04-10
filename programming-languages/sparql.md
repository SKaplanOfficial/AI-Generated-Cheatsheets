# SPARQL Cheatsheet

## Unique Features
- Query language for retrieving data from RDF graphs
- Supports graph pattern matching and filtering
- Can be used to query data from the semantic web
- Based on RDF and RDF Schema standards
- Can be extended with user-defined functions and operators

## Basic Query Structure
```sparql
SELECT ?variable_name
WHERE {
  // Query pattern
}
```

## Triple Patterns
```sparql
subject_predicate_object
```

## Query Modifiers
```sparql
LIMIT limit_value
OFFSET offset_value
ORDER BY variable_name
```

## Filtering
```sparql
FILTER condition
```

## Optional Patterns
```sparql
OPTIONAL {
  // Optional pattern
}
```

## Union
```sparql
{
  // Pattern 1
}
UNION {
  // Pattern 2
}
```

## Grouping and Aggregation
```sparql
SELECT ?variable_name (aggregate_function(?variable_name) AS ?aggregate_variable_name)
WHERE {
  // Query pattern
}
GROUP BY ?variable_name
```

## User-Defined Functions
```sparql
PREFIX my_functions: <http://example.org/my_functions#>

SELECT ?variable_name
WHERE {
  // Query pattern
  FILTER my_functions:function_name(?variable_name)
}
```

## Resources
- [SPARQL 1.1 Query Language](https://www.w3.org/TR/sparql11-query/)
- [SPARQL by Example](https://www.cambridgesemantics.com/blog/semantic-university/sparql-by-example/)
- [Apache Jena](https://jena.apache.org/) (Java framework for working with RDF and SPARQL)
- [RDFLib](https://rdflib.readthedocs.io/) (Python library for working with RDF and SPARQL)