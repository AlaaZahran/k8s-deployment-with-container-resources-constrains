
# Project Title

Create  three redis servers  in finance namespace using k8s deployment with container resource constrains.





## Description
This project aims to create three pods of redis server and  limit resources for these pods in finance namespace .

* Pods specification:

  * image : redis

  * name : redis

  * port : 6379


* Pods resources  :

  * minimum value for pod :
     
     * cpu: 1
     * memory : 1 Gi

  * maximum value for pod:
      
       * cpu : 5
       * memory : 2 Gi
 
## Deployment

To deploy this project run

```bash
  kubectl apply -f redis-deployment.yml 

```


## Check

 To check pods in finance namespace 

```bash
  kubectl get po -n finance
```
    