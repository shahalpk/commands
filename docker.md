
To start a container using `docker-compose` synchronously. It'll stream the logs into console. If you interrupt the command (Ctrl-C), the container will stop. Adding `--build` will build the container if not already built.

    docker-compose -f compose-db.yml up --build
    
To start a container in daemon mode, so it runs in the background.

    docker-compose -f compose-db.yml up -d --build
    
To force recreate a container and start in daemon mode.

    docker-compose -f compose-db.yml up -d --build --force-recreate
    
To start already built containers.

    docker-compose -f compose-db.yml start


## Logs

To tail and stream (with last 10 lines) logs of all the containers in `compose-db.yml` file. Note the `-f` flag in two places, both have different meanings. One is after the `logs` keyword, it's for streaming the file.

    docker-compose -f compose-db.yml logs -f --tail=10

To tail (with last 10 lines) logs of all the containers in the default compose file (`docker-compose.yml`).

    docker-compose logs -f --tail=10
