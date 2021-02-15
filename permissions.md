
- Permissions exist in Task class already.

- type_d.level
    - 0-99 is reserved for non-admin stuff.
    - 100-998 is for admin related stuff.
    - 999 is reserved for super admins: no limitations.
- type_d.metadata.permissions
    - Should contain a list of permissions for this user type.
    - Permissions should match the NAMED ROUTE parameter.
