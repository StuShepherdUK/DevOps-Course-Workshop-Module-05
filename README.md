# Workshop Module 05

This repository is for learners on Corndel's DevOps apprenticeship.

Before the workshop you should complete all the set-up instructions in [before_you_start.md](./before_you_start.md).

During the workshop you'll be following the instructions in [during_the_workshop.md](./during_the_workshop.md).


## Docker Commands (Learning)

#### Build Commands
docker build -f Dockerfile.cliapp -t cliapp .
docker build -f Dockerfile.webapp -t webapp .

#### Run commands
docker run --mount type=volume,source=shared_vol,destination=/opt/chimera/data --detach cliapp
docker run --mount type=volume,source=shared_vol,destination=/opt/chimera/data --detach --publish 80:80 webapp

#### Remove all stopped containers
docker container prune

#### Remove images
docker image list
docker image rm <container>
docker image prune

#### Quick, complete system pruning (caution)
docker system prune (--filter 168h)