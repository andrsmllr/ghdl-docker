# ghdl-docker
A dockerfile to create a docker image for the GHDL open source VHDL simulator.  
Dockerfile for image [andrsmllr/ghdl-{mcode,llvm,gcc} on dockerhub](https://cloud.docker.com/repository/docker/andrsmllr/ghdl-llvm).  

## Usage:

./run.sh [options]  
Will run the docker container like an executable, similar to invoking ghdl when GHDL is installed on your system.  
The current working director will be added to the container by default.  
If files from other paths than the working directory are needed, you have to add these paths using the -v (--volume) option of docker.  

./run_interactive.sh  
Will run the docker container in interactive mode within the current directory.  
Inside the container GHDL can be invoked with the ghdl command.  
The source code is stored under /usr/src.  
