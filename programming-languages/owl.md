# OWL Cheatsheet

## Unique Features
- Formal ontology language for representing knowledge in a machine-readable format
- Based on Description Logic, a subset of first-order logic
- Supports rich modeling of concepts and relationships between them
- Used in artificial intelligence, bioinformatics, and semantic web applications

## Classes
```owl
Class: class_name
```

## Properties
```owl
ObjectProperty: property_name
DatatypeProperty: property_name
AnnotationProperty: property_name
```

## Individuals
```owl
Individual: individual_name
```

## Class Expressions
```owl
Class: class_expression_name
EquivalentTo: class_expression
```

## Property Expressions
```owl
ObjectProperty: property_expression_name
EquivalentTo: property_expression
```

## Axioms
```owl
SubClassOf: class_expression1 class_expression2
EquivalentClasses: class_expression1 class_expression2
SubObjectPropertyOf: property_expression1 property_expression2
EquivalentObjectProperties: property_expression1 property_expression2
```

## Annotations
```owl
AnnotationProperty: annotation_property_name
AnnotationAssertion: annotation_property_name(individual_name "annotation_value")
```

## Resources
- [OWL Web Ontology Language Guide](https://www.w3.org/TR/owl-guide/)
- [OWL 2 Web Ontology Language Primer](https://www.w3.org/TR/owl2-primer/)
- [Protégé](https://protege.stanford.edu/) (ontology editor and development environment)
- [OWL API](https://github.com/owlcs/owlapi) (Java library for working with OWL)