# App python en docker

```bash
docker build . -t fortiz/quotes

docker run -p 8080:80 -e POSTGRES_USER=user -e POSTGRES_PASSWORD=test -e POSTGRES_HOST=localhost -e POSTGRES_DATABASE=quotes fortiz/quotes

docker compose up

curl localhost:8080/quote
```