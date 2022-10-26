### Reloader

Updste pods when ConfigMaps, Secrets, Deployments, etc change

Deploy Reloader 
```
oc apply -f https://raw.githubusercontent.com/stakater/Reloader/master/deployments/kubernetes/reloader.yaml
```

Have it reload when any changes
```
kind: Deployment
metadata:
  annotations:
    reloader.stakater.com/auto: "true"
spec:
  template:
    metadata:
```

More at the [Reloader](https://github.com/stakater/Reloader) GitHub page.

