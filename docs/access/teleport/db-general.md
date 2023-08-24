# Accessing PostgreSQL using Teleport

There are two ways to access PostgreSQL using Teleport:

- The Teleport Connect Client
- The Teleport TSH Client

!!! tip
    
    In both ways, Teleport will forward a port on localhost to the database server.
    You can the use **any** local tools to connect to the forwarded port.

## Prerequisites

- Teleport Connect or TSH Client installed on your local machine. See [Client Installation](/access/teleport/client-installation/) for instructions.
- Client is signed in to Teleport

## Using Teleport Connect Client
Launch the Teleport Connect Client and sign in with your account.

Choose the register `Databases` and select `Connect` and the username to connect to the desired database server.

![Teleport Connect Database](../../assets/images/teleport_connect_database.png)

After that you will see the forwarded port in the Teleport Connect Client.

!!! note "You can manually set the port, if you do not want a random port to be assigned."

![Teleport Connect Database](../../assets/images/teleport_connect_database2.png)

Now you can connect with any database client to the forwarded port using the username displayed in the Teleport Connect Client and no password.

## Using the TSH Client

```bash
# Make sure you are signed in to Teleport
tsh status

# List available databases
tsh db ls

# Connect to a database
tsh db login [--db-user=<user>] [servername]
tsh db connect [--db-user=<user>] [servername]
```

Now you can connect with any database client to the forwarded port using the username displayed in the TSH Client and no password.

