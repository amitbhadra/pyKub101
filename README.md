# Set up Docker Container

```
cd pyKub
docker-compose build python
docker-compose up python
```

Now go to **localhost:5000** and you can see your web app!

In a different terminal - No need to do this since it's already up:

```
docker login docker.io
docker-compose push python
```


# Set up Kubernetes

```
kubectl apply -f kubernetes/deployments/deployment.yml
kubectl get nodes
kubectl apply -f kubernetes/deployments/deployment.yml
kubectl get deploy
kubectl get pods
kubectl apply -f kubernetes/services/service.yml
kubectl get svc
```

Now go to **localhost**, and you will see your web app!