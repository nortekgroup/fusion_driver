# Docker image onfiguration

The file `fastrtps-profile.xml` disabled SharedMemory transport within the docker image that runs nucleus_node. SharedMemory currently prevents the ros2 communication from within the docker container to the host computer. Disabling SharedMemory and instead communicating through UDB allows for the ros communication to occur between the docker container and its host machin