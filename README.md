# tf-k8s - Terraform generating a Kubernetes cluster

Install aws-iam-authenticator

**Initialize terraform**

> terraform init

**Apply IAC script**

> terraform apply --auto-approve

**Setup kubectl to access the cluster generated**

>cp kubeconfig ~/.kube/config

**Use it**

>kubectl get nodes
>kubectl create deploy nging --image=nginx
>kubectl port-forward pod/<nginx-pod-name> 8181:80
