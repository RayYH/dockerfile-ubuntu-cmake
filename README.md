# Ubuntu cmake

Compile and run a c/c++ project via cmake tool.

## `docker run`

```bash
$ docker run -it --name cmake-project -v /path/to/project:/code:rw -d rayyounghong/ubuntu-cmake:latest
$ docker exec -it cmake-project /bin/bash
```

## `docker-compose`

```yml
version: '3'
services:
  cmake-project:
    image: rayyounghong/ubuntu-cmake:latest
    container_name: cmake-project
    volumes:
      - .:/code
    working_dir: /code
    tty: true
    stdin_open: true
```
