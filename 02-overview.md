## K8s Overview

### containers
    - docker: run components in separate containers
    - containers are completed isolated envs w/same os kern underneath
    - OS share same kernal - Linux.  Windows doesnt
        - unlike Hypervisors
    - containers vs VMs
        - containers run on underlying OS
        - VMs have own OS - takes up more space
    - run docker by using image stored in repos like dockerhub
    - containers vs images
        - img is a packge or tmplate to convert. contain 1 or more containers

### orchestration
    - what id containers rely on other containers? how do you run? scale up or down?
    - automatically deploying and managing containers is orchestration
    - ex: docker swarm, Kubernetes, Mesos
    - supported on cloud - AWS/GCP/Azure
    - advantages - HA, load balanced, 
    - uses config files

### Architecture
    - concepts
        - node: machine, worker machine, physical or virtual
        - cluster: set of nodes grouped together
        - master: a node with K8s installed and configured as mster. watches manages other notes
            - components of master: api server, etcd, kubelet, container runtime, controller, scheduler 
        - 