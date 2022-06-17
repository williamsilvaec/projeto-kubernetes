## Listar todos os pods

    kubectl get pods

## Outra forma de ver as informações dos pods

    kubectl get pods -o wide

## Para detalhar as informações de um pod

    kubectl describe pod <nome do pod>

## Excluir um pod

    kubectl delete pod <nome do pod>

## Excluir um pod declarativo

    kubectl delete -f <nome do arquivo>.yaml

## Excluir todos os pods

    kubectl delete pods --all

## Excluir todos os servicos
    
    kubectl delete svc --all

## Criar um deployment

    kubectl apply -f <nome do arquivo>.yaml 

## Exibir o histórico de um deployment

    kubectl rollout history deployment <nome do deployment> 

## Alterar o Change-cause de um deployment

    kubectl annotate deployment <nome do deployment> kubernetes.io/change-cause="<descrição da causa>"

## Voltar um deployment para uma revisão específica

    kubectl rollout undo deployment <nome do deployment> --to-revision=<versão a ser retornada>