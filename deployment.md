We have to create namespaces for different app to deploy so that it will be in one group

![image](https://user-images.githubusercontent.com/92623347/233857323-4f3ee24b-7162-4e84-876c-c370dbb3198b.png)

then we have to create a configuration file  pod.yml file to create a pod



![image](https://user-images.githubusercontent.com/92623347/233867040-6835810f-a8d8-46b0-b698-7ee0eefd7cbb.png)

![image](https://user-images.githubusercontent.com/92623347/233867064-f5a22d93-6957-4e72-bc14-33d9b8fe1096.png)

and in worker node when we get into that container our application django-todo-app will be running

![image](https://user-images.githubusercontent.com/92623347/233867321-1f798e05-88e0-4e90-8d3b-fea6ebc4020f.png)

when we kill that container now it autoheals and creates a new pod automatically

![image](https://user-images.githubusercontent.com/92623347/233867778-a131580f-e0f7-49e1-b831-be8b7bf28b51.png)

![image](https://user-images.githubusercontent.com/92623347/233867828-4a3c3dc5-de32-45bf-8886-0c8de31cdb4e.png)

To replicate pods we need to make deployment file as 
![image](https://user-images.githubusercontent.com/92623347/233869949-955c37f6-e84e-4e89-9f7d-4d8a835d7ad5.png)


![image](https://user-images.githubusercontent.com/92623347/233869973-6fa53999-0580-4c75-bd38-96e9c1a567d6.png)

so 3 replicas are created as mentioned in deployment file

if we want more or less we can aslo change in deployment file configuration according to traffic.









