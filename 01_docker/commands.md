- docker pull
- docker run
- docker run --name my-db -e POSTGRES_PASSWORD=secret -d -p 5432:5432 
postgres:bookworm (to run potgresql)
- docker run -d redis (run in detached mode so your container stays running even when erminal is closed)
- docker ps

- docker stop <id of the container>
- docker start <id of the container>

- dokcer ps -a (see all the containers running or not running)

Pull and run another version of the same image
- docker run redis:4.9 (pulls the image and starts it)

- docker run -p6000:6379 redis (to map ports)