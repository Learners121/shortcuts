[Return to maine page](../readme.md)

# Install postgres

```
# Create the file repository configuration:
    sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'

# Import the repository signing key:
    wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -

# Update the package lists:
    sudo apt-get update

# Install the latest version of PostgreSQL.
# If you want a specific version, use 'postgresql-12' or similar instead of 'postgresql':
    sudo apt-get -y install postgresql
```

# Switch to postgres

```
    sudo -i -u postgres (then use)
    psql -U postgres -W
```

# List of all databases

```
    \l
```

# Select the database

```
    \c database name
```

# List all the tables

```
    \dt
```

# Change the user password

```
    ALTER USER postgres PASSWORD 'Password'
```

# Create the database

```
    create database dbname;
```

# Add data to database

```
    pg_restore --dbname=database_name --verbose database_file
```

# Describe table

```
    \d tablesName
```

# Rename table

```
    ALTER TABLE table_name RENAME TO new_name
```

# Add column in table

```
    ALTER TABLE table_name
    ADD COLUMN column_name data_type
```

# Select statement

it will return the data from the database

```
   SELECT column_names FROM table_name;
   eg
   SELECT first_name FROM customer;
```

# Concat two columns with alias

```
   SELECT first_name || ' ' || last_name AS full_name FROM customer;
```

# Sort data
