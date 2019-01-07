| ID | Target | Description |
|----|--------|-------------|
| ingress-targets-service | Ingress | Makes sure that the Ingress targets a Service | 
| cronjob-has-deadline | CronJob | Makes sure that all CronJobs has a configured deadline | 
| container-resources | Pod | Makes sure that all pods have resource limits and requests set. The --ignore-container-cpu-limit flag can be used to disable the requirement of having a CPU limit | 
| container-image-tag | Pod | Makes sure that a explicit non-latest tag is used | 
| container-image-pull-policy | Pod | Makes sure that the pullPolicy is set to Always | 
| statefulset-has-poddisruptionbudget | StatefulSet | Makes sure that all StatefulSets are targeted by a PDB | 
| deployment-has-poddisruptionbudget | Deployment | Makes sure that all Deployments are targeted by a PDB | 
| pod-networkpolicy | Pod | Makes sure that all Pods are targeted by a NetworkPolicy | 
| networkpolicy-targets-pod | NetworkPolicy | Makes sure that all NetworkPolicies targets at least one Pod | 
| pod-probes | Pod | Makes sure that all Pods have bot a readinessProbe and a libenessProbe configured | 
| container-security-context | Pod | Makes sure that all pods have good securityContexts configured | 
| service-targets-pod | Service | Makes sure that all Services targets a Pod | 
| service-type | Service | Makes sure that the Service type is not NodePort | 
| stable-version | all | Checks if the object is using a deprecated apiVersion | 