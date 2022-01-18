# kubevela-demo

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
kubectl create namesapce testing
kubectl apply --namespace testing --filename dt-full.yaml
```