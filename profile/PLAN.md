## The Plan

Multiple docker containers for all the things I need

### Services

Just docker and a few scrips... 

#### Scripts [(code)](https://github.com/drygnet-homeserver/scripts)
[smee.io](https://smee.io) -client to proxy webhook calls from github when new code and config is pushed

[adnanh/webhook](https://github.com/adnanh/webhook) to react on the webhook calls

Run the scrips as services (use [pm2](https://pm2.io/))

#### Containers

* nginx reverse proxy [(code)](https://github.com/drygnet-homeserver/www)
    
    To route traffic from internet to the web-GUIs of the apps that have GUIs
    
* portainer [(code)](https://github.com/drygnet-homeserver/portainer)
    
    To manage the containers on the server

* MongoDB [(code)](https://github.com/drygnet-homeserver/mongodb)
    
    For all of the apps I will build 😎
    
* mongodb-express [(code)](https://github.com/drygnet-homeserver/mongo-express)
    
    To manage MongoDB
    
* Uptime kuma
   
    To monitor services
    
* Guacamole

    For remote management
    
* AdGuard Home

    For ad-blocking and local dns(?)

    
    
* dev-server
    
    A dynamic but opinionated backend that stores data in mongo 
    
* docker compose for other apps I may need will be here

    ... and will be deployed by the scripts like everything else 
    
* apps developed by me

    for fun and profit (I wish)
