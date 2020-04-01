Here I am deploying my own registry and pushing images to that registry.

Steps (you have to be in the chapter-2 folder for these commands to work)

1. docker-compose up -d
2. docker build -t localhost:5000/mynode-app:1.0 .
3. docker push localhost:5000/mynode-app:1.0
4. curl -XGET http://localhost:5000/v2/_catalog
