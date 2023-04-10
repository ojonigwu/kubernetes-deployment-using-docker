# kubernetes-deployment-using-docker for ubuntu 20.04

step 1 install ubuntu 20.04 server 
       apt update & upgrade 
       apt install ansible
       
step 2 Installs Docker on the target servers
Adds the current user to the Docker group
Adds the Kubernetes repository and installs kubeadm, kubelet, and kubectl
Initializes the Kubernetes control plane and sets up the kubectl configuration
Installs the Calico pod network
then Saves the kubeadm join command for future use 
Make sure to replace inventory.yaml with your inventory file, and kubernetes-installation.yaml with the filename of the playbook

To join a worker node to a Kubernetes cluster that was initialized on a master node, you can use the kubeadm join command. Here's an example Ansible playbook that performs the join process


