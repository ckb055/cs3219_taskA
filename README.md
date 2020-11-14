# Deploy webserver with Nginx and Docker

1. Download repo into a file and navigate to the file directory using your command line.
2. Type `docker build -t reverse proxy .` in the file directory in the command line to start creating an image of our reverse proxy. You can either click on Images in the docker app or run `docker images`. You should see our custom reverseproxy image.
3. Next we run the command `docker-compose up -d` that makes use of our image previously created. We can check that it is working by either clicking on Container in the docker app or run `docker ps -a`
4. In your web browser, go to localhost:8080 and localhost:8081 and we should be able to see different 2 web severs with the help of our reverseproxy webserver.