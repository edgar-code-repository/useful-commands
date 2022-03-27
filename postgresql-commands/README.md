POSTGRESQL COMMANDS
-----------------------------------------------------------------------

Using PostgreSQL from a terminal.

-----------------------------------------------------------------------

**Change password to postgres user**

```

sudo -u postgres psql

ALTER USER postgres PASSWORD '<new_password>';

\q

```
-----------------------------------------------------------------------

**Login to Postgre database**

```

psql -h <host> -d <db> -U <user> -W

```
-----------------------------------------------------------------------

**Listing tables in the database**

```

\dt

```

-----------------------------------------------------------------------
