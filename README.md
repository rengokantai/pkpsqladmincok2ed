#### pkpostsqladmincok
- cp1
```
SELECT inet_server_port();
SELECT current_database();
SELECT current_user;
```

enable remote connection:  

postgresql.conf:
```
listen_addresses = '*'
``` 

==
.pgpass file.
```
			host:port:dbname:user:password
such as		myhost:5432:postgres:user:pass
```

- cp2
```
SELECT date_trunc('second',current_timestamp - pg_postmaster_start_time()) as uptime;
```
