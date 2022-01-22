# kubevela-demo

For more examples, see also: https://github.com/oam-dev/samples

## Install
```
helm repo add kubevela \
    https://kubevelacharts.oss-cn-hangzhou.aliyuncs.com/core

helm repo update

helm upgrade --install \
    kubevela kubevela/vela-core \
    --namespace vela-system \
    --create-namespace \
    --wait
```

```
kubectl apply --namespace vela-system --filename components.yaml
kubectl apply --namespace vela-system --filename traits.yaml
```
## Deploy

```
kubectl create namespace testing
kubectl apply --namespace testing --filename demo-app.yaml
kubectl apply --namespace testing --filename full-demo-app.yaml
```
