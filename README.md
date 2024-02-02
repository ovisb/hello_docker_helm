# Hello Docker Helm chart

Purpose of this helm chart is to help me deploy sample .NET hello-docker app to Kubernetes, and to practice some Azure.

## Pre requirements

In order to install chart you need the following installed:
- helm package
- kubernetes cluster
- access to the ACR which you may not have / or may not exist in the future ^^

## Stand alone installation

```bash
git clone https://github.com/ovisb/hello_docker_helm.git

cd 'hello_docker_helm'

helm install 'hello-docker' 'charts/hello-docker'
 ```

## Uninstall 
```bash
helm delete 'hello-docker'
```

## Integration with ArgoCD
You can check my other repo in the [argocd](https://github.com/ovisb/azure-terraform-v1/tree/main/terraform/argocd) folder.