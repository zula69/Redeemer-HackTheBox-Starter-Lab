# Redeemer-HackTheBox-Starter-Lab


## Objective

The objective of the Redeemer machine is to introduce basic enumeration and exploitation of Redis, an in-memory database. The goal is to connect to the Redis service, explore stored data, and retrieve the flag using command-line interaction.


### Skills Learned
- Basic network scanning (using tools like Nmap)
- Understanding the Redis service and its default port (6379)
- Interacting with Redis using redis-cli
- Enumerating key-value databases
- Identifying misconfigured services (no authentication)
- Extracting sensitive data from a database


### Tools Used
- Kali Linux - used as the attacker PC
- Nmap – used to scan open ports
- redis-cli – used to interact with Redis server
- openvpn - used to connect to HTB environment

## Steps

### Step 1 -connet to the HTB network via openvpn
![vpn](https://github.com/user-attachments/assets/68ad126b-b085-4e2a-8e3a-06eee80e01ff)

### Step 2 -verify connectivity
![ping](https://github.com/user-attachments/assets/4e77c0af-915b-4e18-91b2-34d2f16ebcc2)

### Step 3 -Enumerate the Target
![basicnmap](https://github.com/user-attachments/assets/471989e4-936f-4946-ab29-989cf92eaed2)

- When i do basic nmap scan all basic 1000 ports were closed, so i tried specific port (port 6379) scan which runs the redis service.
  
 ![nmap advanced](https://github.com/user-attachments/assets/b9ee26b4-a643-4813-9d6b-f1c410c39e39)

### step 4 -Installing redis tools
![installing redistools](https://github.com/user-attachments/assets/2405801b-e966-4218-8bb9-ae3271dfdaaa)
![rediscli2](https://github.com/user-attachments/assets/55d64eb2-79cb-4b64-bed7-e1953c5dff2f)


### Step 5-Connect to target using redis-cli
![connecting to the target using redis](https://github.com/user-attachments/assets/192fb2ab-ae2d-4fed-8132-48c827aaf4a8)


### step 6 -use info to return the information and statics of the redis server
![redisinfo](https://github.com/user-attachments/assets/e08e51d0-117c-45ec-8c2e-8008756f34ca)


### step 7-Select the database and view the keys using select and keys *
![keyspaces](https://github.com/user-attachments/assets/c1c63524-87b4-4441-985e-db5f1c20d712)

- The keyspace section provides statistics on main dictionary of each database.

### Step 8-capture the flag
![flag](https://github.com/user-attachments/assets/ae27d629-d3ac-4e6f-ac93-837bdff06d03)

