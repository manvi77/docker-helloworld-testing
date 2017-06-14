# docker-helloworld-testing
builds the local images, -f to point to docker-compose.test.yml and -p to indicate a specific project name:  
docker-compose -f ~/hello_world/docker-compose.test.yml -p ci build  

Run containers, -d to run in the background:    
docker-compose -f ~/hello_world/docker-compose.test.yml -p ci up -d  

Check the output of the sut container by executing:  
docker logs -f ci_sut_1
