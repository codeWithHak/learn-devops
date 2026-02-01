
## Basics

COPY means start from this base image.

And what actually happens is when you build an image it actually builts a new mini computer in your computer whichyou cant see or acceess, but it is on your local machine, but hidden.

So we do port mapping so we can create a way of communication to that port and see that in our browser.

## Volume:

This is crazy by using volume you can actually create a window btw your laptopn and that mini computer you build so whenever you change a file in your laptop that mini computer is able to see and reflect it.

**Before Volume:**
docker run -d -p800:80 static-html
Had to rebuild the image on every change.

**Before Volume:**
docker run -d -p8000:80 -v ${PWD}:/usr/share/nginx/html/index.html static-html

**Debugging Containers**
docker logs <container-name> or <container_id>

Enter inside the mini computer (container)
```docker exec -it 81d70f6d1362 /bin/bash```

Remove everything that's not running:
docker system prune

When you are just testing things out, use the --rm flag in your run command:
docker run --rm -p 8000:80 static-html
The Magic: As soon as you stop this container (or hit Ctrl+C), Docker automatically deletes the container. Now you can go straight to docker rmi without the "Conflict" error.