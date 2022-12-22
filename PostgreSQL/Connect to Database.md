# Connect To Database

Open the terminal, run one of the following commands

### without username and password

```
psql postgres
```

### enter username and password

```
psql -U root -W postgres
```

### enter username and no password

```
psql -U root postgres
```

<br/>

> _root_ is username  
> _postgres_ is a database  
> -U and -W must be uppercase. They are required if we want to connect using username and password
