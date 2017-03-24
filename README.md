# Drunken Lizard Kube

What is the Drunken Lizard Kube?

Kubernetes files for the drunken lizard application.

## Service

Creating the service in kubernetes.

```sh
$ kubectl create -f drunken-lizard-service.yaml
```

## Application

Creating the application controller in kubernetes.

Replace the `DRUNKEN-LIZARDS_TAG` with the latest commit sha that was used to
build the docker image that will be deployed.

```sh
$ kubectl create -f drunken-lizard-controller.yaml
```
