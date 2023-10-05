## usar um namespace para todas as pedalada:

```bash
kubectl config set-context --current --namespace=kafka
``````


```bash
kubectl patch svc kafdrop-service -p '{"spec":{"externalTrafficPolicy":"Cluster"}}'
````

## Engenharia reversa de um item do k8s:

```bash
kubectl get services service_name_interessado -o yaml > nome_do_arquivo_de_saida-yaml
``````