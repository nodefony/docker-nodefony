# docker-nodefony

[![dockeri.co](http://dockeri.co/image/nodefony/docker-nodefony)](https://hub.docker.com/r/nodefony/docker-nodefony/)


Docker Image for nodefony


## What is nodefony?

Nodefony is Node.js full-stack web framework.

Nodefony can be used to develop a complete solution to create a web application.

The Nodefony project is inspired by the PHP Symfony framework, a developer can find most of the concepts, configurations and patterns of Symfony framework.

Nodefony is not an exhaustive port of symfony, nodefony add services like:

 - Web servers (websocket(s), http(s)).
 - Notion of real-time context in Action Controller (Websocket).
 - Notion of synchronous or asynchronous execution in Action Controller (Promise).


# How to use image nodefony Docker ?

docker pull nodefony/docker-nodefony


### exposing  ports

docker run  --rm -it -p 127.0.0.1:5151:5151  -p 127.0.0.1:5152:5152   --name=nodefony nodefony/docker-nodefony

Then you can hit http://localhost:5151 or https://localhost:5152 in your browser.


### exposing  ports ( macosx )


[https://docs.docker.com/docker-for-mac/networking](https://docs.docker.com/docker-for-mac/networking)



# How to use image nodefony Docker with composer  ?

In this mode nodefony run with : 
 
 - docker nginx in front  
 - docker mariadb database  


```bash
$ git clone https://github.com/nodefony/nodefony.git

$ cd nodefony

$ make docker-compose

```

When done : 

Then you can hit http://localhost:5151 or https://localhost:5152 in your browser.


or edit your /etc/hosts  and add entry docker.nodefony

```
##
# Host Database
#
# localhost is used to configure the loopback interface
##

127.0.0.1       localhost docker.nodefony

```

Then you can hit http://docker.nodefony:5151 or https://docker.nodefony:5152 in your browser.


