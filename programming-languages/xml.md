# XML Cheatsheet

## Unique Features
- Markup language for creating structured documents
- Self-describing data format
- Supports user-defined tags
- Hierarchical structure with parent-child relationships
- Widely used in web development and data exchange

## Elements
```xml
<element_name attribute_name="attribute_value">
  Element content
</element_name>
```

## Attributes
```xml
<element_name attribute_name="attribute_value">
  Element content
</element_name>
```

## Comments
```xml
<!-- Comment text -->
```

## Processing Instructions
```xml
<?instruction_name instruction_data?>
```

## Entities
```xml
<!ENTITY entity_name "entity_value">
```

## Namespaces
```xml
<namespace_prefix:element_name xmlns:namespace_prefix="namespace_URI">
  Element content
</namespace_prefix:element_name>
```

## Document Type Definition (DTD)
```xml
<!DOCTYPE root_element_name [
  <!ELEMENT element_name (child_element_name)>
  <!ATTLIST element_name attribute_name attribute_type "default_value">
]>
```

## Resources
- [XML Tutorial](https://www.w3schools.com/xml/)
- [XML in a Nutshell](https://www.oreilly.com/library/view/xml-in-a/0596007647/) (book)
- [XML Validator](https://www.xmlvalidation.com/)
- [XML Editors](https://xml-editors.github.io/) (list of XML editors)