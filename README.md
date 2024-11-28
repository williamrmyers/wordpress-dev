# Dev environemnt for wordpress

currently using docker compose to build and host the environment, which pulls the `wp-content` data into the folder `content`. That should be a seperate repo-which will contain changes to themes and plugins.

The content file should be created withing this folder manually if you are using Fedora with Podman


### Get started
```
mkdir content
chmod 777 content

docker compose up -d
```