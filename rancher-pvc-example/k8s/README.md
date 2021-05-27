# k8s yaml Persistent Volume mount example

This is a complete working example on how to mount local path in the k8s node as a Rancher pvc into a container deployed with kubectl.


## Usage

Enter the correct node name in pv.yaml.<br>
The node name can be checked with:<br>
```kubectl get nodes```

Deploy the yaml files:<br>
```
kubectl create -f storageclass.yaml 
kubectl create -f pv.yaml 
kubectl create -f pvc.yaml 
kubectl create -f deployment.yaml 
```

