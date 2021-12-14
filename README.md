# openserarch_k8s_deployment
Deploy multinode cluster in k8s using helm
# Add the Helm repository
helm repo add opensearch https://opensearch-project.github.io/helm-charts/
# Run the helm install command three times once for each custom YAML file.
1. helm install opensearch-master opensearch/opensearch -f  master.yaml
2. helm install opensearch-data opensearch/opensearch -f  data.yaml
3. helm install opensearch-client opensearch/opensearch -f  client.yaml
