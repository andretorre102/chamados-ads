# chamados-ads - API de Gerenciamento de Chamados

Projeto desenvolvido de forma incremental para a disciplina de **Programação Web** do curso de **Análise e Desenvolvimento de Sistemas (ADS)** da **Universidade Federal do Cariri (UFCA)**, ministrada pelo professor Jayr Pereira.

O objetivo do projeto será construir uma **API RESTful em Python** para gerenciamento de chamados de suporte técnico (estilo helpdesk), permitindo a abertura, acompanhamento, atribuição e resolução de solicitações de atendimento.

A cada semana da disciplina, iremos incrementar o projeto, com a criação de novas rotas, a geração de interface web com o uso do Flasgger para testar os endpoints e ajudar na elaboração da documentação, especificamente da forma como se segue:

#### Semana 1: ✅
Criar API em Python com GET /, repositório GitHub e README.md (Prazo: 23/11/2026).

> **Status da Entrega**: **Etapa 1 (Configuração Inicial)**  
> Estruturou-se o ambiente de desenvolvimento, o gerenciador de dependências e pacotes moderno, com o uso do (`uv`), bem como a rota inicial de verificação de status com Flask.
> Por fim, com a atualização do repositório, inclusive com a criação do arquivo `uv.lock`, procedemos ao versionamento do repositório usando Git e sua respectiva atualização junto ao Github.



#### Semana 2: 
Implementar cadastro, listagem e consulta por ID de chamados em memória (Prazo: 30/11/2026).

#### Semana 3: 
Completar o CRUD em memória e conferir respostas HTTP (Prazo: 07/12/2026).

#### Semana 4: 
Implementar CRUD persistido em SQLite e atualizar instruções de execução (Prazo: 14/12/2026).

#### Semana 5: 
Validar entradas e padronizar erros de dados inválidos e chamado inexistente (Prazo: 18/01/2027).

#### Semana 6: 
Implementar busca por título, filtros e paginação simples (Prazo: 25/01/2027).

#### Semana 7: 
Adicionar testes dos principais fluxos e concluir documentação da API (Prazo: primeiro dia da Semana 8).

#### Semana 8: 
Entregar API em Python, SQLite, filtros, validações, testes e README.md (30/01/2027).

---

#### Semana 1 - Endpoint Disponível

| Método | Endpoint | Descrição | Retorno de Sucesso (`200 OK`) |
| :---: | :---: | :--- | :--- |
| `GET` | `/` | Rota raiz de teste de funcionamento da API | `{"mensagem": "API funcionando"}` |

## Tecnologias Utilizadas

- **Linguagem**: [Python](https://www.python.org/) (versão `>= 3.14`)
- **Framework Web**: [Flask](https://flask.palletsprojects.com/)
- **Gerenciador de Pacotes e Ambientes**: [uv](https://docs.astral.sh/uv/)
- **Controle de Versão**: Git e GitHub

---

## Como Executar o Projeto Localmente

### Pré-requisitos

Inicialmente é necessário ter o gerenciador `uv` instalado. Caso ainda não tenha, basta instalar via `pip`:
```
pip install uv
```

### 1. Clonar o repositório
```bash
git clone https://github.com/andretorre102/chamados-ads.git
cd chamados-ads
```

### 2. Executar a aplicação
Com o `uv`, não é necessário criar ou ativar o ambiente virtual manualmente — o comando abaixo gerencia as dependências do `uv.lock` e sobe o servidor:

```
uv run flask run
```

Em seguida, confira o servidor iniciando no navegador, inserindo:

**`http:\\localhost:5000`**

---

## Autor

- **André Felipe Silva Torres** — [GitHub](https://github.com/andretorre102)
- Curso de Análise e Desenvolvimento de Sistemas — UFCA
