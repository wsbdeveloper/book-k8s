## Module 1

This module will for necessary interactive with the tech kubernetes.

Lets go.

First time: Lets configure the k8s in the your computer, before execute any files type json or yaml.

before, configuration execute the run mongo in pod.

```bash
kubectl create -f ./mongo.json

# exit command
# pod "name_pod" created
```

if interessed, you can login in pod created

```bash
kubectl exec --stdin --tty mongo-pod -- /bin/bash
```

Awesome, we are inside the pod. Now in path bin/ running the mongo cli.

Let's insert new document in collection

```bash
# insert
db.collectionExemplo.insert({ nome: 'K8s is cool!!'})

# read
db.collectionExemplo.find()
```

---

Now let's delete the pod.

```bash
kubectl delete pod mongo-pod # or your pod name.

# pod "mongo-pod" deleted
```
