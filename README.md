1. docker build -t node-app:0.1 .
2. docker images
3. docker run -p 4000:80 --name my-app node-app:0.1
4. curl http://localhost:4000
5. docker stop my-app && docker rm my-app
6. docker run -p 4000:80 --name my-app -d node-app:0.1
7. docker logs [container_id]
8. cd test
9. ....
const server = http.createServer((req, res) => {
    res.statusCode = 200;
    res.setHeader('Content-Type', 'text/plain');
    res.end('Welcome to Cloud\n');
});
....

10. docker build -t node-app:0.2 .
11. docker run -p 8080:80 --name my-app-2 -d node-app:0.2
12. docker stop $(docker ps -q)
13. docker rm $(docker ps -aq)


