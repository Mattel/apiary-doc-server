# Docker Apiary Doc Sever

This allows you to boot a container specifically for running a local apiary.apib file
creating a doc server running on port `4000`

## Installation

To get started all you need to do is add this to the `docker-compose.yml`

```yml
doc:
  image: sproutling/apiary-doc-server
  volumes:
    - .:/app
  ports:
    - "4000:4000"
```

Then to run the app use `docker-compose up` this will pull the dockerhub container and
start running the doc server locally on port `4000`
