# Workshop Module 05

This repository is for learners on Corndel's DevOps apprenticeship.

Before the workshop you should complete all the set-up instructions in [before_you_start.md](./before_you_start.md).

During the workshop you'll be following the instructions in [during_the_workshop.md](./during_the_workshop.md).


## Run commands

docker run --mount type=volume,source=shared_vol,destination=/opt/chimera/data --detach cliapp

docker run --mount type=volume,source=shared_vol,destination=/opt/chimera/data --detach --publish 80:80 webapp