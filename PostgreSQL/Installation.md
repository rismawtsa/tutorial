# Installation

via homebrew

1. Update homebrew

   If it have not been intalled yet in our machine, please [install](https://brew.sh/) it first.

   ```
   brew update
   ```

2. Install postgreSQL

   ```
   brew install postgresql
   ```

   After the installation, on the terminal will show the caveat,

   ```
   caveats:
   This formula has created a default database cluster with:
   initdb --locale=C -E UTF-8 /opt/homebrew/var/postgresql@14
   For more details, read:
   https://www.postgresql.org/docs/14/app-initdb.html

   To restart postgresql@14 after an upgrade:
   brew services restart postgresql@14
   Or, if you don't want/need a background service you can just run:
   /opt/homebrew/opt/postgresql@14/bin/postgres -D /opt/homebrew/var/postgresql@14
   ```

3. Running the postgre as a background service

   ```
   brew services restart postgresql@14
   ```

4. Connect to database
   ```
   psql postgres
   ```
