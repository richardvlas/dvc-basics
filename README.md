# DVC Basics

Demonstrates how to store data in a remote storage location using DVC as well as how to store model artifacts in a different remote storage location.

This is done by configuring the `.dvc` file manually adding `remote` with the name of remote specified in `.dvc/config` file to the outs section.

```
outs:
- md5: 3215096cb053f1b79d8373f78396d2f9
  size: 24
  path: mymodel.json
  remote: azure-model-store
```