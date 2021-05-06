# Dev environment

## Build

Before building project you have to rename file `docker/keys/bitbucket.example` to `docker/keys/bitbucket`
and put SSH key into it. After that building local environment run `docker-compose build` or run `make build`

## Run envs

There are several options exists to work with local environment

- Run container `make start` or `docker-compose up -d`
- Connect to container with angular project `make frontend` or `docker-compose exec angular bash`
- Run dev server for frontend part `make dev-angular` or `docker-compose exec angular bash -c "ng serve --host=0.0.0.0"`

## .env file

For more comfortable, after pull repository just rename file **.env.example** to **.env** and use it.

### Attributes 

**FRONTEND_PORT** - port for angular dev server (commonly used port 4200)

## Configure IDE

## WebStorm

- open **Run -> Edit Configuration** 
- choose **Attach to Node.js/Chrome**
- set Host as **localhost** and Port as **9229**

## Branch naming

All branches have to start their name from `MOU-XXX`, 
where XXX number of ticket. After that prefix developer can add any other name, if needed.

## Dependencies specifications
https://docs.google.com/document/d/1oEfcPyMMx4Em-zsUl-VKDCHpZDHp-y0QR8NlSPO6P2M/edit
