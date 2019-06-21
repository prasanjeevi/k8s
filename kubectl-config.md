# kubectl config

```
apiVersion: v1
kind: Config
clusters:
- cluster:
    server: https://192.168.56.103:6443
    certificate-authority-data:
  name:
- cluster:
    server:
    certificate-authority:
contexts:
- context:
    cluster:
    user:
  name:
- context:
    cluster:
    user:
    namespace:
users:
- name: 
  username:
  password:
- name:
  client-certificate:
  client-key
- name:
  client-certificate-data:
  client-key-data:
- name:
  token:
current-context:
```

```
$HOME/.kube/config
/etc/kubernetes/admin.config
```

```
export KUBECONFIG=
```

```
kubectl config view
kubectl --kubeconfig=file view

kubectl config get-clusters
kubectl config get-contexts
kubectl config current-context

kubectl config use-context

kubectl config set-cluster --server=
kubectl config set-context --cluster= --user= --namespace=
kubectl config set-credentials --username= --password= --token= --client-certificate= --client-key

kubectl config unset
```
