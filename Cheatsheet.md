1. `kubectl create deployment <name> --image=<image>`: Create a new deployment using a specified Docker image.
2. `kubectl delete deployment <name>`: Delete a deployment by name.
3. `kubectl get pods`: List all running pods in the current namespace.
4. `kubectl get deployments`: List all deployments in the current namespace.
5. `kubectl get services`: List all services in the current namespace.
6. `kubectl get nodes`: List all worker nodes in the cluster.
7. `kubectl get namespaces`: List all namespaces in the cluster.
8. `kubectl describe pod <name>`: Get detailed information about a specific pod.
9. `kubectl describe deployment <name>`: Get detailed information about a specific deployment.
10. `kubectl describe service <name>`: Get detailed information about a specific service.
11. `kubectl describe node <name>`: Get detailed information about a specific worker node.
12. `kubectl create namespace <name>`: Create a new namespace.
13. `kubectl delete namespace <name>`: Delete a namespace and all resources within it.
14. `kubectl apply -f <file.yaml>`: Apply a configuration file to create or update Kubernetes resources.
15. `kubectl rollout status deployment/<name>`: Check the status of a deployment rollout.
16. `kubectl rollout undo deployment/<name>`: Roll back a deployment to a previous revision.
17. `kubectl scale deployment <name> --replicas=<number>`: Scale a deployment up or down by changing the number of replicas.
18. `kubectl logs <pod-name>`: View logs for a specific pod.
19. `kubectl exec -it <pod-name> /bin/bash`: Open a shell inside a specific pod.
20. `kubectl attach <pod-name> -i`: Attach to a running container in a pod.
21. `kubectl cp <pod-name>:<remote-path> <local-path>`: Copy a file from a pod to a local machine.
22. `kubectl get events`: List all events in the cluster.
23. `kubectl top <resource> <name>`: Show CPU and memory usage for a pod, deployment, or node.
24. `kubectl get secrets`: List all secrets in the current namespace.
25. `kubectl create secret generic <name> --from-literal=<key>=<value>`: Create a new secret using a literal value.
