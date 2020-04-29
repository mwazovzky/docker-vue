# Docker commands

## Docker build

```
docker build -t mwazovzky.docker-vue .
```

### Tag image
```
docker build -t mwazovzky.docker-vue .
```

## Docker run
```
docker run mwazovzky.docker-vue
```

### Map ports
```
docker run -p 8080:8080 mwazovzky.docker-vue
```

### Link volumes
```
docker run -p 8080:8080 -v /app/node_modules -v $(pwd):/app -e mwazovzky.docker-vue
```

### Overwrite default command
```
docker run -it mwazovzky.docker-vue npm run test:unit
```

## Docker compose
```
docker-compose up [--build]
```

## Docker exec
run command within running container
```
docker exec -it CONTAINER_ID npm run test:unit
```
