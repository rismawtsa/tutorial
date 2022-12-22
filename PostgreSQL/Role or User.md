# Role/User

### create the role/user with password:

```
CREATE ROLE [ROLENAME] WITH LOGIN PASSWORD [PASSWORD];
```

Example:

```
CREATE ROLE root WITH LOGIN PASSWORD ‘root’;
```

`WITH` is optional

> \*use the strong password instead

### alter role:

```
ALTER ROLE root CREATEDB;
```

### show roles:

get the list of roles

```
\du
```

get the specific role

```
\du [ROLENAME]
```
