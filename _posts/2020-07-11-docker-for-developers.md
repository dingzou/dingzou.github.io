---
title: Docker for Developers
---

# Why Docker

As an agile developer, I want to frequently publish my applications so that deployment becomes a routine. The rationale behind this is that this agility makes the “go-to production” event a normal, frequent, completely mastered event instead of a dreaded disaster that may awake monsters who hit me one week later. On the other hand, it is the Ops team that has to face the user if anything goes wrong in deployment - so they naturally want stability.

Containers make deployment easy. Deploying is as simple as running a new container, routing users to the new one, and trashing the old one. It can even be automated by orchestration tools. Since it’s so easy, we can afford to have many containers serving a single application for increased stability during updates.

If you don’t use containers, Ops need to handle your hosting environment: runtimes, libraries, and OS needed by your application. On the other hand, when using containers, they need one single methodology that can handle the containers you provide no matter what’s inside them. You may as well use .NET Core, Java, Node.JS, PHP, Python, or another development tool: it doesn’t matter to them as long as your code is containerized. This is a considerable advantage for containers when it comes to DevOps.


# Run Docker

- A container is what we eventually want to run and host in Docker. You can think of it as an isolated machine, or a virtual machine if you prefer.
- Any container that runs is created from an image. An image describes everything that is needed to create a container; it is a template for containers. You may create as many containers as needed from a single image.
- Images are stored in a registry. In the example above, the app2 image is used to create two containers. Each container lives its own life, and they both share a common root: their image from the registry.

```
docker run hello-world
```
1. Your command asks Docker to create and run a container based on the hello-world image.
2. Since the hello-world image wasn’t already present on your disk, Docker downloaded it from a default registry, the Docker Hub. More about that later.
3. Docker created a container based on the hello-world image.
4. The hello-world image states that, when started, it should output some text to the console, so this is the text you see as the container is running.
5. The container stopped.

```
docker ps -a
docker logs 48bab7f673b3
docker inspect 48bab7f673b3
docker rm 48bab7f673b3
```

# Create Docker Image
WIP

# Publish Docker Image
WIP




source: Docker for Developers in educative.io
