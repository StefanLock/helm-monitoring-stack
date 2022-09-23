# README

### What is this repository for? ###

A repo that is used to deploy a monitoring stack within Kubernetes.
It utilises Helm to package and roll out several applications such as;

- Grafana
- Prometheus


### How do I get set up? ###

#### Install
1. clone repo
2. cd monitoring-stack-helm
3. __Run:__ `helm install monitoring .`

#### Uninstall
1. cd monitoring-stack-helm
2. __Run:__ `helm uninstall monitoring`

#### Testing
##### Grafana
`kubectl --namespace monitoring port-forward service/grafana 3000:3000`

##### Prometheus
`kubectl --namespace monitoring port-forward svc/prometheus 9090:9090`

### Who do I talk to? ###

* Stefan Lock
