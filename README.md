---
author:
- 'Quang-Ngu Truong'
---

\raggedright
\raggedcolumns
2

x2.4885 cm x4.4885 cm Connect &
`psql -U <username> -d <database> -h <hostname>` Disconnect & `\q` & or:
& `\!` Show system status & `\conninfo`

\addvspace{1.3em}
x2.4885 cm x4.4885 cm List users & `SELECT rolname FROM pg_roles;` Show
current user & `SELECT current_user;` Show current user's permissions &
`\du` List databases & `\l` Show current database &
`SELECT current_database();` Show all tables in database & `\dt` List
functions & `\df <schema>`

\addvspace{1.3em}
x2.4885 cm x4.4885 cm Connect to database & `\c <database_name>` [Create
database](http://www.postgresql.org/docs/current/static/sql-createdatabase.html)
& `CREATE DATABASE <database_name> WITH OWNER <username>;` [Drop
database](http://www.postgresql.org/docs/current/static/sql-dropdatabase.html)
& `DROP DATABASE IF EXISTS <database_name>;` [Rename
database](http://www.postgresql.org/docs/current/static/sql-alterdatabase.html)
& `ALTER DATABASE <old_name> RENAME TO <new_name>;`

\addvspace{1.3em}
x2.4885 cm x4.4885 cm List roles & `SELECT rolname FROM pg_roles;`
[Create
user](http://www.postgresql.org/docs/current/static/sql-createuser.html)
& `CREATE USER <user_name> WITH PASSWORD ’<password>’;` [Drop
user](http://www.postgresql.org/docs/current/static/sql-dropuser.html) &
`DROP USER IF EXISTS <user_name>;` [Alter user
password](http://www.postgresql.org/docs/current/static/sql-alterrole.html)
& `ALTER ROLE <user_name> WITH PASSWORD ’<password>’;`

\addvspace{1.3em}
x2.4885 cm x4.4885 cm List tables in current database & `\dt` Globally
list tables & `\ *.*` [Create
table](http://www.postgresql.org/docs/current/static/sql-createtable.html)
&
`CREATE TABLE <table_name>( <column_name> <column_type>, <column_name> <column_type> );`
[Drop
table](http://www.postgresql.org/docs/current/static/sql-droptable.html)
& `DROP TABLE IF EXISTS <table_name> CASCADE;`

\hhline{>{\arrayrulecolor{DarkBackground}}--}
\addvspace{1.3em}
x2.4885 cm x4.4885 cm [Backup
database](http://www.postgresql.org/docs/current/static/app-pgdump.html)
& `pg_dump <database_name>` [Restore
table](http://www.postgresql.org/docs/current/static/app-pgrestore.html)
& `pg_restore -d <database_name> -a <file_pathway>`

\noalign{\gdef\RowColorName{LightBackground}}
\rowcolor{\RowColorName}
[Export table into CSV
file](http://www.postgresql.org/docs/current/static/sql-copy.html) &
`\copy <table_name> TO ’<file_path>’ CSV` [Import CSV file into
table](http://www.postgresql.org/docs/current/static/sql-copy.html) &
`\copy <table_name> FROM ’<file_path>’ CSV`

\hhline{>{\arrayrulecolor{DarkBackground}}--}
\addvspace{1.3em}
**Debugging:**
[[http://www.postgresql.org/docs/current/static/using-explain.html]{style="color: DarkBackground"}](http://www.postgresql.org/docs/current/static/using-explain.html)

[[http://www.postgresql.org/docs/current/static/runtime-config-logging.html
]{style="color: DarkBackground"}](http://www.postgresql.org/docs/current/static/runtime-config-logging.html)

**Advanced Features:**
[[http://www.tutorialspoint.com/postgresql/postgresql\_constraints.htm]{style="color: DarkBackground"}](http://www.tutorialspoint.com/postgresql/postgresql_constraints.htm)
