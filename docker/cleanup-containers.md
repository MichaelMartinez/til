# Clean up all used containers

1. List all containers: `docker ps -a`
2. Determine if you want to keep any containers
3. If Yes, manually remove: `docker -rm <container>`
4. If no: `docker rm -v $(docker ps -aq -f status=exited)`
5. Remember: for one off containers use the `-rm` flag to automatically delete container 
and associated file system upon exit.
