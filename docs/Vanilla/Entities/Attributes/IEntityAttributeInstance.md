# IEntityAttributeInstance


## Importing the package
It might be required for you to import the package if you encounter any issues (like casting an [Array](/AdvancedFunctions/Arrays_and_Loops)), so better be safe than sorry and add the import.  
`import crafttweaker.entity.AttributeInstance;`

## ZenGetters

| ZenGetter      | GetterMethod        | Return Type                          |
|----------------|---------------------|--------------------------------------|
| attribute      | getAttribute()      | [IEntityAttribute](IEntityAttribute) |
| baseValue      | getBaseValue()      | double                               |
| modifiers      | getModifiers()      | `List<IEntityAttrubuteModifier>`     |
| attributeValue | getAttributeValue() | double                               |


## ZenSetters

| ZenSetter | SetterMethod        | Parameter Type |
|-----------|---------------------|----------------|
| baseValue | setBaseValue(value) | double         |


## Modifier Methods

- `List<IEntityAttrubuteModifier>` getModifiersByOperation(int operation)
- boolean hasModifier([IEntityAttributeModifier](IEntityAttributeModifier) modifier)
- [IEntityAttributeModifier](IEntityAttributeModifier) getModifier(String uuid);
- void applyModifier([IEntityAttributeModifier](IEntityAttributeModifier) modifier);
- void removeModifier([IEntityAttributeModifier](IEntityAttributeModifier) modifier);
- void removeModifier(String uuid);
- void removeAllModifiers();
