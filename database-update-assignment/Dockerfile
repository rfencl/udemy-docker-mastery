docker volume create psql
docker container run -d --name psql1 -e POSTGRES_PASSWORD=mypassword -v psql:/var/lib/postgresql/data postgres:15.1
docker container logs -f psql1
docker container stop psql1
docker container run -d --name psql2 -e POSTGRES_PASSWORD=mypassword -v psql:/var/lib/postgresql/data postgres:15.2
docker container logs -f psql2
docker container stop psql2