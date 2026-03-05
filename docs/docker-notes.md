# Docker Setup Notes

## Docker Version

Client:
Version: 29.2.1

Server:
Version: 29.2.1

## Docker Info

Operating System: Docker Desktop  
Architecture: x86_64  
CPUs: 8  
Total Memory: 3.824GiB  

## Test Container

Command:

docker run hello-world

Result:

Hello from Docker!
This message shows that your installation appears to be working correctly.

## Images Pulled

- hello-world:latest
- postgres:15-alpine

## Postgres Container

Command used:

docker run -d \
  --name pg-prework \
  -e POSTGRES_PASSWORD=prework \
  -p 5432:5432 \
  postgres:15-alpine

## PostgreSQL Startup Logs

Output of docker logs pg-prework:

LOG:  database system is ready to accept connections

## Stop Container

Command used:

docker stop pg-prework

## Restart Container

Command used:

docker restart pg-prework

Output after restart:

LOG:  database system is ready to accept connections