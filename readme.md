# Redis In-Memory DB

docker pull redis 

### Running the image

#### Default Redis image 
``` 
docker run --name redis-server -p 6379:6379 -d redis 
```

#### Advanced image (including json features)
```
docker run -p 6379:6379 --name redis-redisjson redislabs/rejson:latest
```

### Checking the logs 

```
docker logs redis-server -f 
```
### Check if redis is exposed on ur machine 

lsof -t -i:6379

### Redis Cli 

There is no direct client. The easiest i could find is using npm.
 
``` 
npm install -g redis-cli
``` 



Check for the available modules on the server

``` 
info modules
```

