# Ubuntu cmake

A sample yaml file:

```yml
version: '3'
services:
  bash:
    image: rayyounghong/ubuntu-cmake:latest
    container_name: cmake-demo
    volumes:
      - .:/code
    working_dir: /code
    tty: true
    stdin_open: true
```