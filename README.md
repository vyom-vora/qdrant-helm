# Entity-Resolution Qdrant helm chart

## Steps to add the github repo to helm repo
1: Go to settings and click on pages
2: Then select a desired branch and save it so you get a github page which would look something like " https://vyom-vora.github.io/qdrant-helm/"
3: Clone the repo, make desired changes to the files.
4: Follow these steps then:
```bash
helm package .
helm repo index --url https://vyom-vora.github.io/qdrant-helm/ .
```
Once the above commands are executed, push the changes to the branch you selected above for github page.


## Steps to setup Qdrant;


```bash
helm repo add qdrant https://vyom-vora.github.io/qdrant-helm/
helm repo update
helm install er-qdrant qdrant/qdrant
```
## Delete Qdrant
```bash
helm delete qdrant
```


### Enable rolling update on configuration change

To enable rolling update on config map modification set `updateConfigurationOnChange` to true
