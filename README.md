# Udacity Fullstack Nano Degree - Project 6

### Overview
---

The information in this readme provides configuration and connection instructions for development and testing purposes.

### Prerequisites
---

It is assumed that an active connection to the internet will be available at all times. To run this program a web browser is required. To SSH into the server from a local environment access to Terminal is required (MAC Linux) or Command Prompt (Windows).

### SERVER CONFIGURATION

Please see details below requested by Udacity:
```
IP address: 35.178.145.28
SSH Port: 2200
URL: http://dabrahamsapp.ddns.net/
```

Summary of software:
```
Ubuntu 18
Apache 2
Postgresql
libapache2-mod-wsgi
```

Summary of configurations made:
```
ufw allow 2200
ufw allow 80
ufw allow 123
ufw enable

adduser grader
created .ssh in grader home folder
created .ssh/authorized_keys file
chmod 644 authorized_keys 
chmod 700 .ssh

/etc/ssh/sshd_config
- AllowUsers ubuntu grader
- Port 2200
- No passwords
- root disabled
```

List of third-party resources:
```
ubuntu documentation
apache documentation
postgres documentation
ufu documentation
mod-wsgi documentation
python documentation
```

### HOW TO CONNECT
---

Open the terminal application and run;
```
ssh -i /path/to/key/here -p 2200 grader@35.178.145.28
```

You should now be logged into the server.

### HOW TO VIEW
---

Open a browser and visit;
```
http://dabrahamsapp.ddns.net/
```

You should now see the app running on the server.

### License
---

This project is licensed under the MIT License.

### Acknowledgments
---
