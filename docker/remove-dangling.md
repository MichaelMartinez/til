# Removing dangling Docker images

If you find `<none>:<none>` images when you run the `docker images` command, you probably have a dangling image. Remove these images with `docker rmi <hash or name>`. You can also list the dangling images with `docker images -f "dangling=true" -q`, then remove them with `docker rmi $(docker images -f "dangling=true" -q)`

aside:

Running the command `docker images -a` will show many `<none>:<none>` images. These images are usually the parent images of the child image you built or pulled. From conversations on IRC in #docker, these should not be removed. You can prune the amount of images on your machine by removing images that are no longer useful and/or not needed. I find that removing the tagged images greatly reduced the overall amount of `<none>:<none>` images on my machine. Keeping the environment nice and tight will be an on-going challenge. 
