# Wordpress-Kubernetes

wordpress run on kubernetes demo with mysql and phpmyadmin

## Clone this project

     git clone https://github.com/supawarin/Wordpress-Kubernetes.git


## Run project

### 1. Run wp-secret.yaml

     kubectl apply -f wp-secret.yaml
   
check it : kubectl get secret


### 2. Run mysql-wp.yaml

     kubectl apply -f mysql-wp.yaml
   
   
### 3. Run wordpress-deployment.yaml

     kubectl apply -f wordpress-deployment.yaml
   
   
### 4. Run phpmyadmin-wp.yaml

     kubectl apply -f phpmyadmin-wp.yaml
   

Check it : 

     kubectl get pods
   
     kubectl get svc
   
     kubectl get pvc
   

# Wordpress-Kubernetes use Helm chart

## Clone this project

     git clone https://github.com/supawarin/Wordpress-Kubernetes.git
   
## Run project

     helm install wp-test -f values-test.yaml ./
   
   
     helm install wp-dev -f values-dev.yaml ./
   
   
     helm install wp-prod -f values-prod.yaml ./
   
   
   
Go to localhost use NodePort number , example : localhost:31077


   <img width="663" alt="wp1" src="https://user-images.githubusercontent.com/83863431/189277278-0915c29e-5157-4ba4-a8d4-9b186a7df970.png">
   
   
   ![wordpress-language](https://user-images.githubusercontent.com/83863431/189277761-6458b4c6-9513-4069-8efe-3f843c0de640.png)
   
Select language and continue

   ![wordpress-installation-screen](https://user-images.githubusercontent.com/83863431/189277876-770e7fe9-7b20-43db-af48-c23e52a089d9.png)

Set up new user and password

   ![1_trwL4Wne-cAZLlCOiLzgSw](https://user-images.githubusercontent.com/83863431/189278045-b64237a6-4c89-4ff6-a31f-29a5d717130b.png)

   
Login use new user & password


<img width="1403" alt="wp2" src="https://user-images.githubusercontent.com/83863431/189278202-d5a24913-d554-49eb-8e69-6f87a45c2a95.png">

