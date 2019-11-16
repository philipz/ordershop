# OrderShop
Redis as an event store in a microservices architecture.

See https://redislabs.com/blog/use-redis-event-store-communication-microservices for a detailed description.

## Start
- `docker-compose up`

## Test
- `docker run -ti --network ordershop_default -v $(pwd):/app python:3 bash && cd /app`
- `pip3 install -r client/requirements.txt`
- `python3 -m unittest client/client.py`

## Stop
- `docker-compose down`
