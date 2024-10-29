# cnwebsite
Cloud native website using nginx and nice static web pages in a container.

# Build a container

``` sh
docker build -t cnwebsite .
```

# Run the container

``` sh
docker run --rm -d -p 8080:80 --name web cnwebsite
```

* --rm: This flag automatically removes the container when it exits. This is useful for temporary containers.
* -d: This flag runs the container in detached mode, meaning it runs in the background.
* -p 8080:80: This flag maps port 8080 on the host machine to port 80 inside the container. This allows you to access the web server running inside the container on port 8080 of your host machine.
* --name web: This flag assigns the name "web" to the container. This makes it easier to manage and identify the container.

# Browse your new website
Browse http://127.0.0.1:8080
