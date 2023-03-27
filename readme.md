---
icon: home
---
# To Illustrate the Problem

This app is configured to run under `$URL/docs/`.

Run it locally:

```sh
retype watch
```

It loads with the correct URL at [`http://localhost:5000/docs/`](http://localhost:5000/docs/).

When run with Docker, however...

```sh
# build the project
docker build -t retype-example:latest .

# run the app in Docker
docker run --rm -p 8080:80 retype-example:latest
```

...now the app shows up at [`http://localhost:8080/`](http://localhost:8080/) instead of the expected [`http://localhost:8080/docs/`](http://localhost:8080/docs/). The expected URL displays a 404 page.
