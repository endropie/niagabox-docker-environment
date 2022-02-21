# Niagahoster Mockup & BoxBilling on Docker

Here document how to run Niagahoster Mockup & BoxBilling.

## Prerequisites

- Docker Desktop or Docker CLI with Docker Compose installed. Follow this [instructions](https://www.docker.com/get-started) to have Docker on your machine.

## Installaion

- Clone Docker variable environments

```
    git clone https://github.com/endropie/niagabox-docker-environment
```

- Now in landing folder git Clone https://github.com/endropie/niagabox-landing

```
    cd landing
    git clone https://github.com/endropie/niagabox-landing .
```

- Now in boxbilling folder git Clone https://github.com/endropie/niagabox-boxbilling

```
    cd boxbilling
    git clone https://github.com/endropie/niagabox-boxbilling .
```

- Copy `.env.sample` to `.env` file inside root folder and set variable. (OPTIONAL)

```
COMPOSE_PROJECT_NAME=BOXBILLING

MYSQL_DATABASE=boxbilling
MYSQL_USERNAME=boxbilling
MYSQL_PASSWORD=password
MYSQL_ROOT_PASSWORD=secret
```

- Now run `docker-compose up` and let docker build images and containers.
- Browse to (http://localhost) to Landing (Niagahoster mockup)
- Browse to (http://localhost:8004) to check our BoxBilling app, or to (http://localhost:8004/bb-admin) to enter BoxBilling admin console

- For testing please login using this credentials:

```
    Email : admin@gmail.com
    Password : pwd12345
```

- Enjoy..!!
