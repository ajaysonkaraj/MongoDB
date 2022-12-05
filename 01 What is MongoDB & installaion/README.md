
# MongoDB

MongoDB, the most popular NoSQL database, is an open-source document-oriented database. The term ‘NoSQL’ means ‘non-relational’. It means that MongoDB isn’t based on the table-like relational database structure. This format of storage is called BSON ( similar to JSON format). 
## Installation in ubuntu

### Install the dependencies
```bash
   apt update

   apt install dirmngr gnupg apt-transport-https ca-certificates software-properties-common
```
### Add MongoDB GPG Key

Download and add the MongoDB GPG key with the following command
```bash
  wget -qO - https://www.mongodb.org/static/pgp/server-5.0.asc | sudo apt-key add -
```
### Create a list for MongoDB
```bash
  echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
```
Update the local package database.
```bash
   apt-get update
```
Install the MongoDB with the following command.
```bash
  apt-get install -y mongodb-org
```
Start the MongoDB service and enable it to start automatically after rebooting the system.
```bash
  systemctl start mongod
  systemctl enable mongod
```
Now, check the status of the MongoDB service.
```bash
  systemctl status mongod
```


### Creating Administrative MongoDB User
```bash
  mongo
```
