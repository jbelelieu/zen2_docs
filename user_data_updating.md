
# Questions
- Does this need to be at a group or a type level?
    - Leaning towards type.

# Overview
- Have a default universal data set that can be updated.
    - field.is_globally_updatable = true
- Then have group by group specific fields that can also be updated.
    - Add this to type_d.metadata.updatableFields
