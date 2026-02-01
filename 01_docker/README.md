## Containers

Containers are a way to package an application with all the necessary dependencies and configuration.

Containers lives in container repositories, docker containers live inside dockerhub.

**Development Before Containers**
You had to manually clone the repo, create venv, and install all dependencies

**After Docker Development**
One command and you have the ready container to run.

**Technical Explanation Of A Container**
A container is layers of images like:
- OS / linux base image
- Applications layer

**Image VS Container**
Image is the actual package and container is the running version of it.
Running = Container
Artifact Not Running = Image

**Two Containers Are Running On Same Port**
Learn about this if redis is running to containers with diff versions on port 6379, what will happen and what is localhost port.