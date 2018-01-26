# sigterm 
This is an example repo on how to do cleanup during the time between the docker stop command is sent to a container and the actual exit of the process

# Usage
  * `make build` - Build the docker container
  * `make run` - Run the docker container. Notice how when you `ctrl + c` the docker process, the words "Cleanup!" print to the screen before the process actually quits. This shows how its possible to intercept the `SIGTERM` and do work before exiting.