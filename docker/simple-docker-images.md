# Simple Docker Images

> For quick and/or simple scripts that need _dockerization_

1. Start with a base image like Debian or Ubuntu.
2. Start a container: `docker run -it -name <name> --hostname <name> debian bash`
3. `apt-get update`
4. `apt-get install <dependencies>`
5. Then run `docker commit` to create an image: e.g. `docker commit <name> test/<name_image>`
