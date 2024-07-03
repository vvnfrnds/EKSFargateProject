# 2048 App

## Create Fargate profile

```
eksctl create fargateprofile \
    --cluster project-cluster \
    --region us-west-2 \
    --name alb-sample-app \
    --namespace project
```

## Deploy the deployment, service and Ingress

```
kubectl apply -f https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.5.4/docs/examples/2048/2048_full.yaml
```
