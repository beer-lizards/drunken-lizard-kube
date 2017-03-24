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

## Database

To create a database and manage database migrations.

Replace the following placeholders:

The database docker image tag.

DRUNKEN_LIZARD_DATABASE_TAG

The database location.

DATABASE_IP
DATABASE_NAME
DATABASE_PASSWORD
DATABASE_PORT
DATABASE_USERNAME

Create the initial user account.

DRUNKEN_LIZARD_ADMIN_EMAIL
DRUNKEN_LIZARD_ADMIN_PASSWORD_ALGORITHM
DRUNKEN_LIZARD_ADMIN_PASSWORD_HASH
DRUNKEN_LIZARD_ADMIN_SALT
DRUNKEN_LIZARD_ADMIN_USER
