## K8s Setup
- options in building cluster
    - can seteup locally using minikube, microk8s, kubeadm
    - hosted solutions - AWS, GCP, Azure
    - part of course we got cluster through browser
- minikube setup
    - how it works
        - minikube bundles up all components(controller, api server, kubelet, etcd, runtime) into a single image
        - bundle pkged into ISO for download
        - minikube provides .exe to download and install
        - must use VM like virtualbox
        - must have kubectl command line tool installed
- aws setup first: ec2 instance, roles, ssh 
    - ec2 instance created
    - create .pem file and download
    - change permissions chmod 400 <key name>.pem
    - in terminal ssh -i 'k8s.pem' ec2-user@ec2-34-224-80-109.compute-1.amazonaws.com   
- MiniKube setup prereq
    - first need to install Kubectl
        - www.kubernetes.io
        - install and setup kubectl
- install minikube
    - make sure virtualization is enabled for setup
        - use grep to check if virtulization is enabled



