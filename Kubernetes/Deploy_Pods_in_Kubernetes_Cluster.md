# Task
The Nautilus DevOps team is diving into Kubernetes for application management. One team member has a task to create a pod according to the details below:

1. Create a pod named `pod-nginx` using the `nginx` image with the `latest` tag. Ensure to specify the tag as `nginx:latest`.<br/>
2. Set the app label to `nginx_app`, and name the container as `nginx-container`.<br/>

Note: The kubectl utility on `jump_host` is configured to operate with the Kubernetes cluster.

## Solution

Create a pod yaml file.

```sh
vi pod-nginx.yaml
```

```yml
apiVersion: v1
kind: Pod
metadata:
  name: pod-nginx
  labels:
    app: nginx_app
spec:
  containers:
  - name: nginx-container
    image: nginx:latest

```

Deploy pod.

```sh
kubectl apply -f pod-nginx.yaml
```

Check if pod is running.

```sh
kubectl get pods
NAME        READY   STATUS    RESTARTS   AGE
pod-nginx   1/1     Running   0          4m46s
```
## References

[Pods](https://kubernetes.io/docs/concepts/workloads/pods/)

<br/><br/>
[back](https://github.com/harshitsahu2311/KodeKloud-Engineer-Tasks)  
