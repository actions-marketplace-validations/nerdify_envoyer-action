# Envoyer Action

> GitHub Action for triggering a deployment on [Envoyer](https://envoyer.io)

## Usage

```workflow
workflow "Deploy Envoyer" {
  on = "push"
  resolves = ["deploy"]
}

action "deploy" {
  uses = "nerdify/envoyer-action@master"
  secrets = ["ENVOYER_DEPLOY_URL"]
}
```

## Secrets

* `ENVOYER_DEPLOY_URL` - **Required**. Deployment url.