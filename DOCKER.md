# Docker commands

### Docker build
```
docker build -t mwazovzky.docker-vue .
```

### Docker run
```
docker run -p 8080:8080 mwazovzky.docker-vue
docker run -p 8080:8080 -v /app/node_modules -v $(pwd):/app -e mwazovzky.docker-vue
```

### Docker compose
```
docker-compose up [--build]
```
