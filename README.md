# NEXUS
IITG Intranet Chat Web App

[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/IITGSocialIntranet/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link)

## Installation

Steps for setting up Nexus:

Installing Npm and Node.js:
```
$ sudo apt-get update
$ sudo apt-get install nodejs
$ sudo apt-get install npm
```

Installing and configuring MongoDB  [here](https://www.howtoforge.com/tutorial/install-mongodb-on-ubuntu-16.04/)(till step 4).
```
$ mongo
> use nexus
```

Generate SSL Certificate:
```
$ openssl genrsa 2048 > ssl.pem
$ openssl req -new -key ssl.pem -out csr.pem
$ openssl x509 -req -days 365 -in csr.pem -signkey ssl.pem -out ssl.crt
```

Launching Nexus:
```
$ sudo npm install --save
$ sudo npm install -g nodemon
$ nodemon server.js
```

## ScreenShots
#### Login
![Login Page](/Screenshots/login.png "Login Page")
#### First time user details set up
![Initial Details](/Screenshots/details.png "Initial Details")
#### Uploading profile pic
![Profile Pic Upload](/Screenshots/profilepicupload.png "Profile Pic Upload")
#### Personal Messaging
![Personal Message](/Screenshots/personalmessage.png "Personal Message")
#### Search bar
![Search](/Screenshots/search.png "Search")
#### Creating new room for group chat
![Room Create](/Screenshots/roomcreate.png "Room Create")
#### Add user to the new room
![Room Add user](/Screenshots/addpeople.png "Room Add user")
#### Room chats
![Room Chat](/Screenshots/roomchat.png "Room Chat")
