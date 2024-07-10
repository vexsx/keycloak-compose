### [Keycloak](https://github.com/keycloak/keycloak) with MSSQL

1. Requires [docker](https://docs.docker.com/get-docker/) and [compose](https://docs.docker.com/compose/install/)
2. Parameterized using variables in the [`.env`](.env) file
3. Up the project using command:
```
docker compose up -d
```

| App | Port | Username | Password
|-|-|-|-
| Keycloak | http://localhost:8080 | `admin` | `keycloak`


| Useful commands | Description
|-|-
| `docker stats` | Containers resource usage (`--no-stream` only pull the first result)
| `docker compose logs` | Shows logs of containers (`-f` to follow logs)
| `docker compose down` | Stop and remove containers (`-v` remove named volumes declared in the volumes section of the Compose file and anonymous volumes attached to containers)
| `docker system prune -a -f` | Remove all unused containers, networks, images (`--volumes` prune volumes)
