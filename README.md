```
   ______              __           __
  /\__  _\          __/\ \__       /\ \
  \/_/\ \/     ___ /\_\ \ ,_\      \_\ \
     \ \ \   /' _ `\/\ \ \ \/      /'_` \
      \_\ \__/\ \/\ \ \ \ \ \_  __/\ \L\ \
      /\_____\ \_\ \_\ \_\ \__\/\_\ \___,_\
      \/_____/\/_/\/_/\/_/\/__/\/_/\/__,_ /
```

Batch scripts for Ruby production environment install on Ubuntu Server.

[![wercker status](https://app.wercker.com/status/2dd2ff58518cae2dd75e4556e6d931c5/s/master "wercker status")](https://app.wercker.com/project/bykey/2dd2ff58518cae2dd75e4556e6d931c5)

## Requirements

* Ubuntu Server 14.04

## Usage

Install packages first

```bash
sudo apt-get update
sudo apt-get install -y curl
curl -sSL https://coding.net/u/taff/p/init.d/git/raw/master/install_packages | bash
```

### Install Nginx

Nginx [official package](http://nginx.org/packages/ubuntu/)

```bash
curl -sSL https://coding.net/u/taff/p/init.d/git/raw/master/install_nginx | bash
```

### Install RVM + Ruby

```bash
curl -sSL https://coding.net/u/taff/p/init.d/git/raw/master/install_rvm | bash
```

Use Ruby China mirror site for RubyGems and Ruby:

```
MIRROR=1 curl -sSL https://coding.net/u/taff/p/init.d/git/raw/master/install_rvm | bash
```

### Install MongoDB

```bash
curl -sSL https://coding.net/u/taff/p/init.d/git/raw/master/install_mongodb | bash
```

### Install Redis

```bash
curl -sSL https://coding.net/u/taff/p/init.d/git/raw/master/install_redis | bash
```

### Install ElasticSearch

```bash
curl -sSL https://coding.net/u/taff/p/init.d/git/raw/master/elasticsearch | bash
sudo service elasticsearch status
```

## Install Docker

```bash
curl -sSL https://coding.net/u/taff/p/init.d/git/raw/master/install_docker | bash
sudo docker info
```
