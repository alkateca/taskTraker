# taskTraker

Baseado no projeto disponível em: [roadmap.sh](https://roadmap.sh/projects/task-tracker)
(último acesso em 02/12/2025)

Rastreador de tarefas (Task tracker) é um projeto usado para acompanhar e gerenciar tarefas. 
Nesta projeto, você construirá uma interface CLI para acompanhar o que você precisa fazer, 
o que você já fez e no que você está trabalhando. 

## Requisitos
A aplicação deve ser executada a partir da linha de comando, 
aceitar ações e entradas do usuário como argumentos e 
armazenar as tarefas em um arquivo JSON . 

O usuário deve ser capaz de:

* Adicionar, Atualizar e Excluir tarefas

* Marcar uma tarefa como em progresso ou concluída

* Listar todas as tarefas

* Listar todas as tarefas que estão concluídas

* Listar todas as tarefas que não estão concluídas

* Listar todas as tarefas que estão em progresso

## Exemplo 

Lista de comandos e suas funções devem ser da seguinte forma:

bash

```
# Adicionando uma nova tarefa
task-cli add "Comprar mantimentos"
# Saída: Tarefa adicionada com sucesso (ID: 1)
# Atualizando e excluindo tarefas
task-cli update 1 "Comprar mantimentos e preparar o jantar"
task-cli delete 1
# Marcando uma tarefa como em progresso ou concluída
task-cli mark-in-progress 1
task-cli mark-done 1
# Listando todas as tarefas
task-cli list
# Listando tarefas por status
task-cli list done
task-cli list doing
task-cli list to-do
```

## Propriedades das tarefas

Cada tarefa deve ter as seguintes propriedades:

* id: Identificador único

* description: Descrição breve

* status: O status da tarefa (todo, in-progress, done)

* createdAt: Data de criação

* updatedAt: Data de mudança