## Guia de Contribuição

| Data       | Versão | Descrição            | Autor(es)                                |
| ---------- | ------ | -------------------- | ---------------------------------------- |
| 29/04/2023 | 1.0    | Criação do documento | [@gpersijn](https://github.com/gpersijn) |

### 1. Idioma

<p align="justify">
Durante todo o desenvolvimento deve-se utilizar inglês para nomes de variáveis, nome de diretórios, nome de arquivos e código em geral. Já para texto de commits, texto de Issues e texto de pull request deve-se utilizar o português.</p>

### 2. Padrão de commit

<p align="justify">
O padrão de commit deve seguir o seguinte formato: '#' + numero da Issue + ' - ' + texto, conforme o exemplo abaixo:</p>

Para código de desenvolvimento/testes:

```
git commit -m "#12 - adicionando funcionalidade x"
```

Para documentação, deve-se utilizar o seguinte formato:

```
git commit -m ":docs: #12 - adicionando texto x"
```

Para atualizações de tarefas de configuração, sem alterações no código:

```
git commit -m "chore: mudando na sidebar"
```

### 3. Padrão de Issue

Cada desenvolvedor ao criar uma Issue deve:

- Iniciar com template de Issue disponibilizado
- Colocar assignees
- Colocar as tags de desenvolvimento
- Escrever no template de Issue os tópicos de acordo com a tarefa

```

<!-- Certifique-se de ser uma tarefa bem contida. Certifique-se da possibilidade de desmembrar a issue em issues melhores e, caso seja possível, o faça  -->
# Descrição:
<!-- Dê os objetivos da issue, para quê serve, qual issue afeta, que artefato é criado/alterado. Ao citar outras issues, utilize o código delas: #Número_da_issue -->
Essa issue tem como objetivo realizar uma ...

# Tarefas:
<!-- Não economize na listagem de tarefas -->
- [x] Adicionar tópico 1 - @fulano
- [x] Adicionar tópico 2 - @fulano
- [ ] Adicionar tópico 3 - @fulano

# Critério de aceitação:
<!-- O revisor da issue deve marcar esses critérios antes de fechá-la -->
- [x] Documento markdown criado
- [x] O documento já deve estar no gitpages

```

### 4. Padrão de Pull Request

<p align="justify">
O padrão de pull request segue o template proposto pelo github, preenchendo os tópicos de:</p>

- Descrição
- Mudanças
- Screenshots (opcional)
- Issue

### 5. Padrão de documentação

<p align="justify">
Ao criar um novo documento markdown certifique-se que o padrão de documentação siga:

```
## Titulo do documento

| Data       | Versão | Descrição            | Autor(es)                                |
| ---------- | ------ | -------------------- | ---------------------------------------- |
| xx/xx/xxxx | 1.0    | Criação do documento | [@usuario](https://github.com/usuario) |

### 1. Tópico 1

<p align="justify">
texto texto texto
</p>

```
