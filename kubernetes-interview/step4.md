### Task
Artifactory base charts are located at [here](https://github.com/jfrog/charts/tree/master/stable/artifactory-oss). Review the README and then use Helm to install Artifactory OSS.

`helm repo add jfrog https://charts.jfrog.io`{{execute}}

`helm install artifactory-oss --set postgresql.postgresqlPassword=password --namespace artifactory jfrog/artifactory-oss `{{execute}}

 
