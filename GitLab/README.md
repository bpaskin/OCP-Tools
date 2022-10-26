### GitLab on OCP

1. Install the operator
```
oc apply -f install-gitlab-operator.yaml
```
2. Update the `create-gitlab-instance.yaml` with the proper Cluster Domain in place of `DOMAIN_NAME_HERE`
3. Create an instance
```
oc apply -f create-gitlab-instance.yaml
```

