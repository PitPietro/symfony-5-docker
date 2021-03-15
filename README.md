# Symfony 5 Docker
Following Martin Pham's [Symfony 5 development with Docker](https://dev.to/martinpham/symfony-5-development-with-docker-4hj8) tutorial on [dev.to](https://dev.to).

## Project structure
```bash
|-- docker
|   |-- database/
|   |   |-- data/
|   |   |-- Dockerfile
|   |
|   |-- logs/
|   |   |-- logs/
|   |   |   |-- nginx/ # added a .gitkeep file to push this emppty folder
|
|   |-- nginx/
|   |   |-- nginx.conf
|   |   |-- Dockerfile
# TODO fix this in a most readable way

```

## Create the Symfony project
It is already created for you, but, in case you would like to re-do in again.

```bash
# remove the 'src' folder
rm -rfv src
# create the symfony project inside the 'src' folder
symfony new src
```

## Run the docker
```bash
cd docker

docker-compose up
```

Let's open [http://localhost](http://localhost), you should see the default page of Symfony 5.

## Reference
1. [commit and push an empty git folder](https://www.devopsroles.com/how-to-commit-and-push-an-empty-git-folder/)