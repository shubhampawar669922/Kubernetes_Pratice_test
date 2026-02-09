# Kubernetes Pratice Test

## Q1. What is the smallest unit that Kubernetes deploys?

A. Node

B. Pod

C. Service

D. Container

Ans - Pod

## Q2. Which Kubernetes object is used to expose pods to network traffic?

A. Pod

B. Deployment

C. Service

D. Namespace

Ans - Service

## Q3. Which Service type is used only for internal communication inside the cluster?

A. NodePort

B. LoadBalancer

C. ClusterIP

D. ExternalName

Ans - ClusterIP

## Q4. You want to access an application using <NodeIP>:<Port>

Which Service type should you use?

A. ClusterIP

B. NodePort

C. LoadBalancer

D. Headless

Ans - NodePort

## Q5. Which Service type is mainly used in cloud environments to expose applications externally?


A. ClusterIP

B. NodePort

C. LoadBalancer

D. ExternalName

Ans - LoadBalancer

## Q6. A pod is deleted accidentally. Which pod type can automatically recreate it?

A. Standalone Pod

B. Static Pod

C. Pod managed by Deployment

D. Init Pod

Ans - Pod managed by Deployment

## Q7. Which pod type is used to run initialization tasks before the main container starts?

A. Sidecar Pod

B. Init Pod

C. Static Pod

D. Multi-container Pod

Ans - Init Pod

## Q8. Containers inside the same pod communicate using:

A. Different IP addresses

B. Service only

C. Same IP address

D. External LoadBalancer

Ans - Same IP address

## Q9. Which Service assigns a stable internal IP address automatically?

A. NodePort

B. LoadBalancer

C. ClusterIP

D. ExternalName

Ans - ClusterIP

## Q10. You created a Service, but traffic is not reaching the pod.
What is the most common reason?

A. Wrong image

B. Label mismatch

C. Pod crash

D. Node failure

Ans - Label mismatch

## Q11. Which Kubernetes component provides DNS-based service discovery?

A. kubelet

B. kube-proxy

C. CoreDNS

D. Scheduler

Ans - CoreDNS

## Q12. You want a pod to always run on a specific node.
Which pod type is used?

A. Init Pod

B. Sidecar Pod

C. Static Pod

D. Ephemeral Pod

Ans - Static Pod

## Q13. Which Service type exposes a fixed port on every node?

A. ClusterIP

B. NodePort

C. LoadBalancer

D. ExternalName

Ans - NodePort

## Q14. You want pods inside the cluster to access an application using a DNS name.

Which Service type should you use?

A. NodePort

B. LoadBalancer

C. ClusterIP

D. ExternalName

Ans - ClusterIP

## Q15. Which command shows the IP address of a pod?

A. kubectl get nodes

B. kubectl logs pod

C. kubectl get pods -o wide

D. kubectl describe service

Ans - kubectl get pods -o wide

## Q16. You created a LoadBalancer Service in a local cluster.
What usually happens?

A. External IP is assigned immediately

B. External IP stays pending

C. Pod is deleted

D. Service creation fails

Ans - External IP stays pending

## Q17. Which pod type is commonly used to support a main application with logging or monitoring?

A. Init Pod

B. Standalone Pod

C. Sidecar Pod

D. Static Pod

Ans - Sidecar Pod

## Q18. Which Service field decides which pods receive traffic?

A. ports

B. type

C. selector

D. metadata

Ans - selector

## Q19. Which command is used to list all Services in a namespace?

A. kubectl get pods

B. kubectl get svc

C. kubectl describe pod

D. kubectl logs svc

Ans - kubectl get svc

## Q20. Two pods in the same namespace want to communicate.
What is the recommended Kubernetes way?

A. Use pod IP directly

B. Use Service name

C. Use node IP

D. Use external IP

Ans - Use Service name

# Pratical Assignment

## Task
You are given an application image that runs a web server.

Perform the following steps:

Create a Deployment that runs the application with at least 2 pods.

Ensure all pods are created successfully and are in Running state.

Create a NodePort Service to expose the application.

Access the application from a browser using:

    http://<NodeIP>:<NodePort>

Verify that the application output is visible in the browser.

Take a screenshot of the browser output.

Create a README.md file and add:

Deployment name

K8s task

Service type used

URL used to access the application

Screenshot of the browser output

Push the K8s task README.md file to a Git repository and submit the repository link.

Ans - 

1. web-app-deployment

2. NodePort

3. http://54.167.52.237:30007/

4.
 ![new-1](./images/new-1.png)