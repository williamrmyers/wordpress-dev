# Dev environemnt for wordpress

currently using docker compose to build and host the environment, which pulls the `wp-content` data into the folder `content`. That should be a seperate repo-which will contain changes to themes and plugins.

The content file should be created withing this folder manually if you are using Fedora with Podman

add a `.env` file and following.
```
MYSQL_ROOT_PASSWORD=example
MYSQL_DATABASE=example
MYSQL_USER=example
MYSQL_PASSWORD=example

WORDPRESS_DB_HOST=db:3306
WORDPRESS_DB_USER=example
WORDPRESS_DB_PASSWORD=example
WORDPRESS_DB_NAME=example
```


### Get started
```
mkdir content
chmod 777 content

docker compose up -d
```