<p align="center">
   <a href="https://github.com/isiroca/docker-dev-env/network"><img src="https://img.shields.io/github/forks/isiroca/docker-dev-env.svg" alt="GitHub forks"></a>
   <a href="https://github.com/isiroca/docker-dev-env/issues"><img src="https://img.shields.io/github/issues/isiroca/docker-dev-env.svg" alt="GitHub issues"></a>
   <a href="https://raw.githubusercontent.com/isiroca/docker-dev-env/master/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="GitHub license"></a>
</p>

# DockerDevEnv

Docker PHP Development Environment

## Tools

DockerDevEnv include:

* Apache2
* Composer
* Laravel
* Memcached
* Mongo
* NodeJs
* MySQL
* NGINX
* PHP 5.6 
* PHP 7.0 
* PHP 7.1
* PHPMyAdmin
* Python
* Redis
* Symfony
* XDebug

## Getting Started

### Prerequisites

What things you need to install DockerDevEnv?

* [Docker](https://docs.docker.com/engine/installation/)
* [Docker Compose](https://docs.docker.com/compose/install/)
* [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)


### Installing

#### Clone this repo

```
git clone https://github.com/IsiRoca/docker-dev-env.git
```

#### Copy env-example

Copy env-example file. 

```
cd docker-dev-env
cp env-example .env
```

#### Edit .env

Then edit .env file and put your own config.

For example, you can install MongoDB editing the variables to TRUE.

```
WORKSPACE_INSTALL_MONGO=true
PHP_FPM_INSTALL_MONGO=true
```

Or maybe install Python

```
WORKSPACE_INSTALL_PYTHON=true
```

#### Start DockerDevEnv

The next commands install DockerDevEnv.

If you only need install NGINX and MySQL, then run this command.

```
docker-compose up -d nginx mysql
```

If you prefer install NGINX, MySQL, PHPMyAdmin and Redis

```
docker-compose up -d nginx mysql phpmyadmin redis
```

#### Docker Containers

Show all DockerDevEnv Containers

```
docker ps -a
```

Access to Workspace Container

```
docker exec -ti workspace bash
```


## Author

- [Isi Roca](https://github.com/isiroca) @isiroca | [Twitter](https://twitter.com/IsiRoca) | [Site](http://isiroca.com)


## License

[MIT License](https://github.com/IsiRoca/docker-dev-env/blob/master/LICENSE)
