# Problem Statement
> Write a simple python program, that would expose itself to port 80 with HELLO SCRIBETECH message. Then, write yaml manifest for it, deploy it to K8S and expose it using nginx ingress. Create a Canary and blue-green deployment for it. This Pod should load before Nginx (you need to prove this)

Steps:
  1. `kubectl apply -f nginx.yaml`
  2. `kubectl port-forward service/nginx 30000:8090`
  3. open http://localhost:30000
