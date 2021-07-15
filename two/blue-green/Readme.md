# Problem Statement
> Create a deployment running nginx version 1.16.1 that will run 2 pods that uses /var/www as its root dir. Nginx should run on port 8090. It should mounts a volume and the volume should have a dir /var/www and contain a file "Hello SCRIBETECH" html

Steps:
  1. `kubectl apply -f nginx.yaml`
  2. `kubectl port-forward service/nginx 30000:8090`
  3. open http://localhost:30000