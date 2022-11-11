# STORAGE CLASS - PERSISTENT VOLUME CLAIM - PERSISTENT VOLUME OLUSTURMA

- rbac.yaml ==> provisioner pod için yapılacak yetkilendirmeler (sa,role,rolebindings)
- nfs_class.yaml ==> storage class
- nfsdeployment.yaml ==> provisioner pod oluşturacak deployment
- test_nfs_pvc_dynamic.yaml ==> test amaçlı bir pvc oluşturmak için,

```
kubectl apply -f rbac.yaml
kubectl apply -f nfs_class.yaml
kubectl apply -f nfsdeployment.yaml
kubectl apply -f test_nfs_pvc_dynamic.yaml
```
