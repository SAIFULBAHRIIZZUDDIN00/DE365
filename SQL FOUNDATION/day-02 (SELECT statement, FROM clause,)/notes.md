SELECT *
FROM SAIFUL;

SELECT retrieves data from a database.

* asterisk means all columns.
FROM keyword followed by the table name.
SAIFUL is the name of the table we are requesting data from.
; we end the statement with a semicolon.

# Specific Columns
The * grabs all the columns in a table, but what if we want to select just a few of the columns?

If we only want to select specific columns, we can list out the column names, separated by commas:

SELECT column1, column2, column3
FROM table_name;

Here’s an example:

SELECT id, name, genre
FROM shows;

We only select the id, name, and genre columns from the shows table.

Note: SQL keywords like SELECT and FROM are not case-sensitive, but it's common to write them in uppercase to distinguish them from column names (id, name, genre) and table names (shows), which are written in lowercase.

REFERENCE:
#CODEDEX#
