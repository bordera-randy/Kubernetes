kubectl create deployment <name> --image=<image>: Create a new deployment using a specified Docker image.
kubectl delete deployment <name>: Delete a deployment by name.
kubectl get pods: List all running pods in the current namespace.
kubectl get deployments: List all deployments in the current namespace.
kubectl get services: List all services in the current namespace.
kubectl get nodes: List all worker nodes in the cluster.
kubectl get namespaces: List all namespaces in the cluster.
kubectl describe pod <name>: Get detailed information about a specific pod.
kubectl describe deployment <name>: Get detailed information about a specific deployment.
kubectl describe service <name>: Get detailed information about a specific service.
kubectl describe node <name>: Get detailed information about a specific worker node.
kubectl create namespace <name>: Create a new namespace.
kubectl delete namespace <name>: Delete a namespace and all resources within it.
kubectl apply -f <file.yaml>: Apply a configuration file to create or update Kubernetes resources.
kubectl rollout status deployment/<name>: Check the status of a deployment rollout.
kubectl rollout undo deployment/<name>: Roll back a deployment to a previous revision.
kubectl scale deployment <name> --replicas=<number>: Scale a deployment up or down by changing the number of replicas.
kubectl expose deployment <name> --type=NodePort --port=<port>: Expose a deployment as a service on a specific port.
kubectl logs <pod-name>: View logs for a specific pod.
kubectl exec -it <pod-name> /bin/bash: Open a shell inside a specific pod.
kubectl attach <pod-name> -i: Attach to a running container in a pod.
kubectl cp <pod-name>:<remote-path> <local-path>: Copy a file from a pod to a local machine.
kubectl get events: List all events in the cluster.
kubectl top <resource> <name>: Show CPU and memory usage for a pod, deployment, or node.
kubectl get secrets: List all secrets in the current namespace.
kubectl create secret generic <name> --from-literal=<key>=<value>: Create a new secret using a literal value.
kubectl delete secret <name>: Delete a secret by name.
kubectl create configmap <name> --from-literal=<key>=<value>: Create a new config map using a literal value.
kubectl delete configmap <name>: Delete a config map by name.
kubectl edit <resource> <name>: Edit a resource in real time.
kubectl label <resource> <name> <key>=<value>: Add a label to a resource.
kubectl annotate <resource> <name> <key>=<value>: Add an annotation to a resource.
kubectl apply -f <dir>: Apply all configuration files in a directory.
kubectl apply -f <url>: Apply a configuration file from a URL.
kubectl delete -f <file.yaml>: Delete all resources in a configuration file.
kubectl delete all --all: Delete all resources in the current namespace.
kubectl exec -it <pod-name> -- <command>: Run a command inside a specific pod.
