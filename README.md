# cardano-daedalus-docker

Docker containers for [Cardano Settlement Layer](https://whycardano.com/) staging and mainnet w/ explorers and [Daedalus](https://daedaluswallet.io/). Also a `docker-compose` file to configure and launch them.

## Docker images

* https://hub.docker.com/r/cloneearth/cardano-sl-mainnet-wallet/
* https://hub.docker.com/r/cloneearth/cardano-sl-mainnet-explorer/
* https://hub.docker.com/r/cloneearth/cardano-sl-staging-wallet/
* https://hub.docker.com/r/cloneearth/cardano-sl-staging-explorer/

## Setup

These images have been tested on Digital Ocean Ubuntu 16.04 x64.

1. Create instance of Ubuntu 16.04 x64 and `ssh` in to it as `root`.
2. Install docker
    * `sudo curl -sSL https://get.docker.com/ | sh`
3. Install docker-compose
    1. ```sudo curl -L https://github.com/docker/compose/releases/download/1.18.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose```
    2. `sudo chmod +x /usr/local/bin/docker-compose`
4. `git clone https://github.com/bigearth/cardano-daedalus-docker.git`
5. `cd cardano-daedalus-docker`
6. `docker-compose up`

## Credits

This project was originally forked from https://github.com/hcvst/cardano-daedalus-docker. Thanks to Hans Christian v. Stockhausen for his work on that repo.
