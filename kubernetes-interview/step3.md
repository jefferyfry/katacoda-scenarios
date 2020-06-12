## Install Artifactory OSS

Artifactory base charts are located at [here](https://github.com/jfrog/charts/tree/master/stable/artifactory-oss). Review the README and then use Helm to install Artifactory OSS.

`helm repo add jfrog https://charts.jfrog.io`{{execute}}

`helm install artifactory-oss --set postgresql.postgresqlPassword=password --namespace artifactory jfrog/artifactory-oss `{{execute}}

### Questions
1. How can I see everything that was installed?
`kubectl get all --namespace=artifactory`{{execute}}
2. How do can we monitor the Helm install?
`kubectl get pods --namespace=artifactory`{{execute}}
3. If you are seeing issues with the deployment how would you investigate?
`kubectl describe pod <pod name> --namespace=artifactory`{{execute}}
4. If you wanted to try again, how would you do that?
`helm delete artifactory-oss`{{execute}}
 
