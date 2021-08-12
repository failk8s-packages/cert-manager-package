# package-cert-manager

This package provides certificate management functionality using [cert-manager](https://cert-manager.io/docs/).

## Components

* cert-manager

## Configuration

The following configuration values can be set to customize the cert-manager installation.

### Global

## Usage Example

This walkthrough guides you through using cert-manager...


## Develop checklist

1. Update your [config.json](./config.json) with the package info
2. Add [overlays](./src/bundle/config/overlays/) and [values](./src/bundle/config/values.yaml)
3. Test your bundle: `ytt --data-values-file src/example-values/minikube.yaml  -f target/bundle/config` providing a sample values file from [example-values](./src/examples-values/)
4. Build your bundle `./hack/build.sh`
5. Publish your bundle: `./hack/push.sh`
6. Add it to the [failk8s-repo](https://github.com/failk8s-packages/failk8s-repo) and publish the new repo and test the package from there, or [test with local files](./target/test)