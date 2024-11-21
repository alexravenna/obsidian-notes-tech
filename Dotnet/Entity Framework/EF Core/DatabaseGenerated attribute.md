---
resources:
  - https://www.learnentityframeworkcore.com/configuration/data-annotation-attributes/databasegenerated-attribute
---
# Description
- Allows EF Core to tell the [[Database|database]] to generate a value for a property upon insertion and update (`[DatabaseGenerated(DatabaseGeneratedOption.Computed)]`) or just upon insertion (`[DatabaseGenerated(DatabaseGeneratedOption.Identity)]`)