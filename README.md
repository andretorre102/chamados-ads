# chamados-ads - API de Gerenciamento de Chamados

## Estudante

- **André Felipe Silva Torres** ([Perfil do GitHub](https://github.com/andretorre102))
- **Matrícula**: 2025012328

Projeto desenvolvido de forma incremental para a disciplina de **Programação Web** do curso de **Análise e Desenvolvimento de Sistemas (ADS)** da **Universidade Federal do Cariri (UFCA)**, ministrada pelo professor Jayr Pereira.

O objetivo do projeto é construir uma **API RESTful em Python** para gerenciamento de chamados de suporte técnico (estilo helpdesk), permitindo a abertura, acompanhamento, atribuição e resolução de solicitações de atendimento.

A cada semana da disciplina, iremos incrementar o projeto, com a criação de novas rotas, a geração de interface web com o uso do [Flasgger](https://github.com/flasgger/flasgger) para testar os endpoints e ajudar na elaboração da documentação, especificamente da forma como se segue:

#### Semana 1: ✅
Criar API em Python com GET /, repositório GitHub e README.md (Prazo: 23/11/2026).

> **Status da Entrega**: **Etapa 1 (Configuração Inicial)**  
> Estruturou-se o ambiente de desenvolvimento, o gerenciador de dependências e pacotes moderno, com o uso do (`uv`), bem como a rota inicial de verificação de status com Flask.  
> Por fim, com a criação do arquivo `uv.lock`, procedemos ao versionamento do repositório usando Git, geração da tag `semana-01` e sua respectiva atualização junto ao GitHub.

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

## Tecnologias Utilizadas

- **Linguagem**: [Python](https://www.python.org/) (versão `>= 3.14`)
- **Framework Web**: [Flask](https://flask.palletsprojects.com/)
- **Gerenciador de Pacotes e Ambientes**: [uv](https://docs.astral.sh/uv/)
- **Controle de Versão**: Git e GitHub

---

## Como Executar o Projeto

### Pré-requisitos

É necessário ter o gerenciador `uv` instalado. Caso ainda não tenha, basta instalar via `pip`:
```bash
pip install uv
```
### 1. Clonar o repositório
```bash
git clone https://github.com/andretorre102/chamados-ads.git
cd chamados-ads
```

### 2. Instalar as dependências
Para sincronizar as dependências exatas registradas no arquivo de bloqueio (`uv.lock`), execute:
```bash
uv sync --locked
```

### 3. Executar a aplicação

#### Ambiente Local:
```bash
uv run flask run
```

#### No GitHub Codespaces:
```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

---

## Endpoints Disponíveis

### Rota Raiz (Verificação de Status)

| Método | Endpoint | Descrição | Retorno de Sucesso (`200 OK`) |
| :---: | :---: | :--- | :--- |
| `GET` | `/` | Retorna o status de funcionamento da API de chamados | `{"mensagem": "API de chamados em funcionamento"}` |

#### Como testar a rota:
Via navegador acessando `http://localhost:5000/`, ou pelo terminal:
```bash
curl -i http://localhost:5000/
```

#### Resposta JSON esperada:
```json
{
  "mensagem": "API de chamados em funcionamento"
}
```

---


