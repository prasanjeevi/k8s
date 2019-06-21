# pod

```
apiVersion: v1
kind: Pod
metadata:
- name:
  namespace:
  labels:
    app:
  annotations:
    buildno:
spec:
  containers:
  - name:
    image:
    
```

```
kubectl run netapiserver --image=netapiserver --restart=Never --dry-run -o yaml


apiVersion: v1
kind: Pod
metadata:
  creationTimestamp: null
  labels:
    run: netapiserver
  name: netapiserver
spec:
  containers:
  - image: netapiserver
    imagePullPolicy: IfNotPresent
    name: netapiserver
    resources: {}
  dnsPolicy: ClusterFirst
  restartPolicy: Never
status: {}
```
