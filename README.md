# sqlserver-docker

docker-compose up -d

docker-compose down


```sql
	create database nortwin

	RESTORE FILELISTONLY 
	FROM DISK = '/var/opt/mssql/backups/AdventureWorks2017.bak';

	RESTORE DATABASE nortwin
	FROM DISK = '/var/opt/mssql/backups/AdventureWorks2017.bak'
	WITH
	MOVE 'AdventureWorks2017' TO '/var/opt/mssql/data/AdventureWorks2017.mdf',
	MOVE 'AdventureWorks2017_log' TO '/var/opt/mssql/data/AdventureWorks2017_log.ldf',
	REPLACE,
	RECOVERY;

	use nortwin

	SELECT * from Person.Address
```
