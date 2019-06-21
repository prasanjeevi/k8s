# deployment

```
kubectl run netapiserver --image=netapiserver --dry-run -o yaml

apiVersion: extensions/v1beta1 # apps/v1
kind: Deployment
metadata:
  creationTimestamp: null
  labels:
    run: netapiserver
  name: netapiserver
spec:
  replicas: 1
  selector:
    matchLabels:
      run: netapiserver
  strategy: {}
  template:
    metadata:
      creationTimestamp: null
      labels:
        run: netapiserver
    spec:
      containers:
      - image: netapiserver
        name: netapiserver
        resources: {}
status: {}
```
