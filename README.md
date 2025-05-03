# Redis with authentication
docker run -d --name redis-stack -p 6379:6379 -p 8001:8001 -e REDIS_ARGS="--requirepass mypassword" redis/redis-stack:latest

# Redis without authentication
docker run -d --name redis-stack -p 6379:6379 -p 8001:8001 redis/redis-stack:latest
