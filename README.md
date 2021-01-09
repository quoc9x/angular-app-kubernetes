## Overview

Project sử dụng Docker và Kubernetes để CI/CD tự động cho nhiều instance của một image.

## Create deployment kubernetes

kubectl apply -f deployment.yaml

## Update image for deployment

kubectl set image deployment/angular-deployment angular=cuongquocvn/angular-app:latest

## Restart deployment kubernetes

kubectl rollout restart deployment angular-deployment
