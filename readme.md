# ORACLE VM
## Files for installing oracle vm 19c
-- To be added

Note: comment out this line in `/etc/security/limits.d/oracle-database-preinstall-19c.conf`
```
oracle hard memlock 134217728
```

Run this as root:
```
chown oracle /opt/oracle/product/19c/dbhome_1/bin/*
```

Run this as oracle:
```
chmod 6751 /opt/oracle/product/19c/dbhome_1/bin/*
```

You need to set env variables as oracle
none of the env variables come up under oracle, none mentioned in Dockerfile.

As oracle:

```
Enter user-name: system
Enter password: 
ERROR:
ORA-01034: ORACLE not available
ORA-27101: shared memory realm does not exist
Linux-x86_64 Error: 2: No such file or directory
Additional information: 4376
Additional information: -1341788829
Process ID: 0
Session ID: 0 Serial number: 0
```