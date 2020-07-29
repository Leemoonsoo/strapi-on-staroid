# strapi on staroid

Deploy your own [strapi](https://strapi.io) server on [staroid](https://staroid.com).

- Postgresql DB
- Configurable instance (CPU/Mem)
- Configurable strapi version
- File browser to manage files
- Shell terminal from web browser


[![Run](https://staroid.com/api/run/button.svg)](https://staroid.com/api/run)


## How to use

 - 1. Click 'Run on Staroid' button and launch an instance
 - 2. Once instance is created, click 'Open' button and create an Administrator
 - 3. Before login, allow public access (otherwise, login will fail)

    ![](https://user-images.githubusercontent.com/1540981/88838719-d0fca180-d18e-11ea-8db8-6a0a40b1b0fb.png)

## Run locally using skaffold with minikube

 - Install [skaffold](https://skaffold.dev)
 - Install [minikube](https://kubernetes.io/docs/tasks/tools/install-minikube/)

```
skaffold dev -f .staroid/skaffold.yaml --port-forward -p minikube
```

Browse

 - localhost:1337 - strapi
 - localhost:8000 - file browser
