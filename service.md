First we need to create a file service.yml

![image](https://user-images.githubusercontent.com/92623347/233873816-531ac986-718d-46e6-bedf-66a73c72d41b.png)

![image](https://user-images.githubusercontent.com/92623347/233873961-891e1308-10ee-4468-a6d1-50f199f182ee.png)
and we need to open port 30007 on worker node so that we can check whether our application runs or not.

![image](https://user-images.githubusercontent.com/92623347/233877147-9d3b15fc-178e-4fb3-aefa-941645f9c29f.png)

according to our traffic we can increase replicas and autoscales automatically and service cretes for that load.

we can see upscaling and downscaling pods and strategy type by giving describe command for deployments.
