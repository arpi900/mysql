notes:

1. MySQL Transaction cannot be able to roll back all statements. For example, these statements include DDL (Data Definition Language) commands such as CREATE, ALTER, or DROP database as well as CREATE, UPDATE, or DROP tables or stored routines. We have to make sure that when we design our transaction, these statements do not include.

2. If a DDL statement, such as CREATE TABLE, immediately follows three INSERT statements, the CREATE TABLE statement executes an automatic COMMIT statement, permanently storing changes to the database made by the INSERT statements. The new rows added can’t be removed from the database using a ROLLBACK statement

