## Unleash Docker with cookie authentication hook

Customization of the [unleash](https://github.com/Unleash/unleash) docker [image](https://github.com/Unleash/unleash-docker) to make it work together with [oauth2-proxy](https://pusher.github.io/oauth2_proxy/). If you set up oauth2-proxy infront of your service in the cluster, you can rely on the oauth2-proxy cookie to retrieve the information about the user.

## Work locally with this repo 
Start by cloning this repository. 

You can use `docker-compose` to start postgres and the unleash server together. This makes it really fast to start up
unleash locally without setting up a database or node.

```bash
$ docker-compose build
$ docker-compose up
```

### Requirements
We are using docker-compose version 3.3 and it requires:

- Docker engine 17.06.0+
- Docker compose 1.14.0+

For more info, check out the compatibility matrix on Docker's website: [compatibility-matrix](
https://docs.docker.com/compose/compose-file/compose-versioning/#compatibility-matrix)