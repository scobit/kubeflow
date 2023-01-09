#### Installation page
https://www.kubeflow.org/docs/started/installing-kubeflow/

Особенности установки 1.6
1
kserving
kserve/kserve-controller:v0.8.0
gcr.io/kubebuilder/kube-rbac-proxy:v0.8.0
 
2
change everywhere and reboot auth ns and istio pods
dex.auth.svc.cluster.local.
 
3
Достуановить ручые манифесты по созданию namespace
 
#### Default Username and Password
user@example.com

12341234

### kubeflow namespaces

#### dex
auth

#### common component cert-manager
cert-manager

#### common component for network 
istio-system

####
knative-eventing
knative-serving

#### example namespace for default user
kubeflow-user-example-com

#### kubeflow itself
kubeflow


### some issue when delete old kubeflow
kubectl get apiservices v1beta1.custom.metrics.k8s.io
kubectl delete APIServices v1beta1.custom.metrics.k8s.io


#### Default username and password for kcell deploy
kubeflow.datalake

5%XeaJ%yt%


#### Image for test notebooks
artifactory.kraken.kcell.kz:6555/datalake-jupyterlab-kubeflow:765


###
kubectl -n kubeflow rollout restart deploy


