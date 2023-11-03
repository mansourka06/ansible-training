# TP-1_ansible inventory and hosts vars

## Actions taken :

- **Create a cluster (1 ansible and 1 client)**.

- **Create a hosts.ini file in .ini format** with the following inventory settings
    * All hosts in the "all" group must be logged in as user admin.
    * The client must belong to a group called "prod".
    * The password for all ssh connections must be admin for all machines in the "prod" group.
    * The "env" variable should be equal to "production" for all machines in the "prod" group.

- **Then create an inventory.yml file**, the yaml version of the .ini file.

- **Test the ad-hoc ping and setup commands with the two inventory files**.

