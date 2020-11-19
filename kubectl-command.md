扩容
```sh
kubectl scale rc kubia --repliaca=3 
```
缩容
```sh
kubectl scale rc kubia --repliaca=2 
```
扩容／缩容
```sh
kubectl edit rc kubia 修改replicas 
```
```sh
kubectl run kubia --image=liksa/kubia --port=8080 --generator=run/v1
```
列出集群中所有的节点
```sh
kubectl get nodes
```
列出集群中所有的pod
```sh
kubectl get pods --all-namespaces
```
查看对象的详细信息
```sh
kubectl describe pod  xxxx -n namespaces
```
k8s 创建容器 
```sh
kubectl create/apply -f  kubia.yml 
```
k8s删除容器
```sh
kubeclt delete pod kubia
```
节点维护
```sh
kubectl cordon node1
```
```sh
kubectl drain node1
```
```sh
kubectl uncordon node1
```

查看pod日志
```
kubectl logs -f --tail=100 nginx
```
进入容器内部
```sh
kubectl exec -it podname /bin/bash
```
