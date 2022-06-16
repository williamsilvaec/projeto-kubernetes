## Listando os pods

    kubectl get pods

## Excluindo um pod

    kubectl delete pod nome_do_pod

## Criando um deployment

    kubectl apply -f nome_do_arquivo.yaml 

## Exibindo o histórico de um deployment

    kubectl rollout history deployment nome_do_deployment 

## Alterando o Change-cause de um deployment

    kubectl annotate deployment nome_do_deployment kubernetes.io/change-cause="descrição da causa"