# strapi on staroid

Deploy your own [strapi](https://strapi.io) server on [staroid](https://staroid.com).

- Postgresql DB
- Configurable instance (CPU/Mem)
- Configurable strapi version
- File browser to manage files
- Shell terminal from web browser


[![Run](https://staroid.com/api/run/button.svg)](https://staroid.com/api/run)

## Run locally using skaffold with minikube

 - Install [skaffold](https://skaffold.dev)
 - Install [minikube](https://kubernetes.io/docs/tasks/tools/install-minikube/)

```
skaffold dev -f .staroid/skaffold.yaml --port-forward -p minikube
```

Browse

 - localhost:1337 - strapi
 - localhost:8000 - file browser
