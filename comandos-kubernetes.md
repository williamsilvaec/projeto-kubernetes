## Listando os pods

    kubectl get pods

## Excluindo um pod

    kubectl delete pod <nome do pod>

## Criando um deployment

    kubectl apply -f <nome do arquivo>.yaml 

## Exibindo o histórico de um deployment

    kubectl rollout history deployment <nome do deployment> 

## Alterando o Change-cause de um deployment

    kubectl annotate deployment <nome do deployment> kubernetes.io/change-cause="<descrição da causa>"

## Voltar um deployment para uma revisão específica

    kubectl rollout undo deployment <nome do deployment> --to-revision=<versão a ser retornada>