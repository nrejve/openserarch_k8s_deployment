# openserarch_k8s_deployment
Deploy multinode cluster in k8s using helm
1. Add the Helm repository
helm repo add opensearch https://opensearch-project.github.io/helm-charts/)
2. Run the helm install command three times once for each custom YAML file.
 helm install opensearch-master opensearch/opensearch -f  master.yaml
 helm install opensearch-data opensearch/opensearch -f  data.yaml
 helm install opensearch-client opensearch/opensearch -f  client.yaml
