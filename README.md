# Entity-Resolution Qdrant helm chart


## Steps to setup Qdrant;


```bash
helm repo add qdrant https://vyom-vora.github.io/qdrant-helm/
helm repo update
helm install qdrant qdrant/qdrant
```
## Delete Qdrant
```bash
helm delete qdrant
```


### Enable rolling update on configuration change

To enable rolling update on config map modification set `updateConfigurationOnChange` to true
