Database setup:

```
postgresql13-server has the following notes:
    To create a database instance, after install do
     sudo mkdir -p /opt/local/var/db/postgresql13/defaultdb
     sudo chown postgres:postgres /opt/local/var/db/postgresql13/defaultdb
     sudo su postgres -c 'cd /opt/local/var/db/postgresql13 &&
    /opt/local/lib/postgresql13/bin/initdb -D
    /opt/local/var/db/postgresql13/defaultdb'

    A startup item has been generated that will aid in starting
    postgresql13-server with launchd. It is disabled by default. Execute the
    following command to start it, and to cause it to launch at startup:
    
        sudo port load postgresql13-server
```
