## Tasks
* []Launch Minikube
* []Deploy pong pod and service using custom `selector`
* []Set ingress route to each application
* []Test nodeport
* []Active pong linkerd proxy


## Commands
### Apply k8s manifest
```
kubectl apply -f [ . | FILE_PATH ]
```

### check LISTEN ports on Mac
`sudo lsof -i -P | grep LISTEN `

### Install nginx ingress controller
```sh
helm upgrade --install ingress-nginx ingress-nginx \
  --repo https://kubernetes.github.io/ingress-nginx \
  --namespace ingress-nginx --create-namespace
```

### Check linkerd dashboard pid
```sh
ps -ef | grep dashboard
```


### Running fastapi app
```
# cd to git clone path
python3 -m venv .
source bin/activate
pip install -r requirements.txt
fastapi dev app/main.py
deactivate
```
