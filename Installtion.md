Creating 2 nodes master and worker in aws .

![image](https://user-images.githubusercontent.com/92623347/233848857-abfab639-acf7-4bd6-aba1-bdcb89feddc7.png)

First we need to update both server and worker using this command 

sudo apt update -y

Next install docker using sudo apt install docker.io -y

start docker using systemctl start docker

and when restarts the system docker should start automatically , we need to use this command
 systemctl enable docker
 
 Next we need kubeadm on both the nodes for that we need to run few commands
 
 ![image](https://user-images.githubusercontent.com/92623347/233850781-3755c970-827e-4e2c-9054-2163cc88238d.png)
 then we have to install kubeadm , kubectl and kubelet
 
 ![image](https://user-images.githubusercontent.com/92623347/233851741-0bbfc2ee-4278-48f5-9829-d40d217d352c.png)
 
 for kubeadm we need to work as a root user otherwise you will get permission issues
 sudo su
 we need to start kubeadm to initiate cluster with
 kubeadm init
 
 ![image](https://user-images.githubusercontent.com/92623347/233852030-402bac64-89d9-4038-b16d-61282febca9b.png)

 
 ![image](https://user-images.githubusercontent.com/92623347/233852195-69565604-3c8d-493a-a4a1-66d0bbfdbeba.png)

we have admin.conf file where we have all the info about cluster
![image](https://user-images.githubusercontent.com/92623347/233852305-7b57bde5-834f-4f13-b418-3b4d0da4cb4a.png)
we need to geta token from master so that we can connect to any worker node

![image](https://user-images.githubusercontent.com/92623347/233852659-87f3f99a-5715-4b0b-ba4e-9fdefe1b0dbc.png)

and we need to give this token to worker node to connect then both are connected with each other
![image](https://user-images.githubusercontent.com/92623347/233853291-f1c980f7-96ca-49c8-8877-2983cfea3081.png)





 


