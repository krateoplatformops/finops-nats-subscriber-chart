# Krateo FinOps NATS Subscriber

This is a [Helm Chart](https://helm.sh/docs/topics/charts/) for [Krateo FinOps NATS Subscriber](https://github.com/krateoplatformops/finops-nats-subscriber).

## Configuration

You must to configure four parameters in the values.yaml file:
 - subTopic: the topic that the subscriber will receive data on;
 - optNamespace: the namespace where the "finops-operator-vm-manager" is deployed;
 - optSecretName: the name of the secret containing the token for the Azure REST API;
 - optSecretNamespace: the namespace of the secret containing the token for the Azure REST API;

## How to install

```sh
$ helm repo add krateo https://charts.krateo.io
$ helm repo update krateo
$ helm install finops-nats-subscriber krateo/finops-nats-subscriber
```
