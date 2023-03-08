# Kubernetes Cheatsheet  
## Basics  
|Command|	Description  |
| --- | --- |
| kubectl version	| Display the Kubernetes version.  |
| kubectl cluster-info	| Display the cluster info.  |
| kubectl get nodes	| List all worker nodes in the cluster.  |
| kubectl get namespaces	| List all namespaces in the cluster. | 

## Pods  
|Command|	Description  | 
| --- | --- |
| kubectl get pods	| List all running pods in the current namespace.  |  
| kubectl describe pod <name>	| Get detailed information about a specific pod.  |  
| kubectl logs <pod-name>	| View logs for a specific pod.  |  
| kubectl exec -it <pod-name> /bin/bash	| Open a shell inside a specific pod.  |  
| kubectl attach <pod-name> -i	| Attach to a running container in a pod.  |  
| kubectl cp <pod-name>:<remote-path> <local-path>	| Copy a file from a pod to a local machine.  |  

## Deployments  
|Command|	Description  |  
| --- | --- |  
|  kubectl get deployments	|  List all deployments in the current namespace.  |  
|  kubectl create deployment <name> --image=<image>	|  Create a new deployment using a specified Docker image.  |  
|  kubectl describe deployment <name>	|  Get detailed information about a specific deployment.  |  
|  kubectl scale deployment <name> --replicas=<number>	|  Scale a deployment up or down by changing the number of replicas.  |  
|  kubectl delete deployment <name>	|  Delete a deployment by name.  |  
|  kubectl rollout status deployment/<name>	|  Check the status of a deployment rollout.  |  
|  kubectl rollout undo deployment/<name>	|  Roll back a deployment to a previous revision.  |  
  
## Services  
|Command|	Description  |  
| --- | --- |  
|  kubectl get services	|  List all services in the current namespace.  
|  kubectl describe service <name>	|  Get detailed information about a specific service.  
|  kubectl expose deployment <name> --type=NodePort --port=<port>	|  Expose a deployment as a service on a specific port.  

## Configurations  
|Command|	Description  |  
| --- | --- |  
|  kubectl apply -f <file.yaml>	|  Apply a configuration file to create or update Kubernetes resources.  |  
|  kubectl apply -f <dir>	|  Apply all configuration files in a directory.  |  
|  kubectl apply -f <url>	|  Apply a configuration file from a URL.  |  
|  kubectl delete -f <file.yaml>	|  Delete all resources in a configuration file.  |  
|  kubectl delete all --all	|  Delete all resources in the current namespace.  |  
|  kubectl edit <resource> <name>	|  Edit a resource in real time.  |  

## Miscellaneous  
|Command|	Description  |  
| --- | --- |  
|  kubectl get events	|  List all events in the cluster.  
|  kubectl top <resource> <name>	|  Show CPU and memory usage for a pod, deployment, or node.  
|  kubectl describe node <name>	|  Get detailed information about a specific worker node.   
|  kubectl get secrets	|  List all secrets in the current namespace.  
|  kubectl create secret generic <name> --from-literal=<key>=<value>	|  Create a new secret using a literal value.  
|  kubectl delete secret <name>	|  Delete a secret by name.  
|  kubectl create configmap <name> --from-literal=<key>=<value>	|  Create a new config map using a literal value.  
