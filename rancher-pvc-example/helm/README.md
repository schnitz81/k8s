# Helm Persistent Volume mount example

This is a complete working example on how to mount local path in the k8s node as a Rancher pvc into a container deployed with Helm.


## Usage

Enter the correct node name in values.yaml.<br>
The node name can be checked with:<br>
```kubectl get nodes```

Deploy Helm chart:<br>
```helm upgrade --debug rancher-pvc-example -f values.yaml -i .```

Delete Helm chart:<br>
```helm del rancher-pvc-example```

