# package-cert-manager

This package provides certificate management functionality using [cert-manager](https://cert-manager.io/docs/).

## Components

* cert-manager

## Configuration

The following configuration values can be set to customize the cert-manager installation.

### Global

## Usage Example

This walkthrough guides you through using cert-manager...


## Develop

```
cd bundle
# Update vendir.yml
vendir sync
# Add overlays and values and update README.md
# Test
ytt -f config
# Lock images used
kbld -f . --imgpkg-lock-output .imgpkg/images.yml
# Publish bundle
imgpkg push --bundle quay.io/failk8s/cert-manager-package:<VERSION> --file .
```