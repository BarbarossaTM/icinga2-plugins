# Check Dell/EMC² Isilon / PowerScale storage systems

This plugin can check Dell/EMC² Isilon / PowerScale storage systems for events/alarms,
the state of the storage pools and SyncIQ replication.

The checks are done via the Platform API (PAPI) and require a valid user with access rights
for the PAPI and some read only priviledges (see below).


## Cluster configuration

For this check to work there needs to exist a user on your cluster with priviledges
to access the Platform API and read only access to the events, smartpools, and synciq (for all feature to work).

This can be done by creating a role like this:

```
# isi auth roles view Monitoring
       Name: Monitoring
Description: -
    Members: imt-monitoring-user
 Privileges
             ID: ISI_PRIV_LOGIN_PAPI
      Read Only: True

             ID: ISI_PRIV_EVENT
      Read Only: True

             ID: ISI_PRIV_SMARTPOOLS
      Read Only: True

             ID: ISI_PRIV_STATISTICS
      Read Only: True

             ID: ISI_PRIV_SYNCIQ
      Read Only: True
```

And then creating a user account (e.g. in the 'local' provider) and assigning the user to the above (or a similar) role.
