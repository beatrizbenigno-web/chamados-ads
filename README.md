# API : CHAMADOS DE SUPORTE

**UFCA - ANÁLISE E DESENVOLVIMENTO DE SISTEMAS**
**Estudante:** Beatriz Benigno de Vasconcelos

## Objetivo do projeto

Primeira API com Flask: criar uma API de chamados de suporte. Nesta etapa, a aplicação expõe apenas a rota inicial, que confirma que a API está no ar.

## Como instalar as dependências

Pré-requisito: ter o Python instalado. Instale o `uv` e, na pasta do projeto, sincronize as dependências com o `uv.lock`:

```bash
pip install uv
uv sync --locked
```

O `uv sync --locked` cria o ambiente virtual (`.venv`) e instala exatamente as versões registradas no `uv.lock`.

## Como executar a aplicação

```bash
uv run flask run
```

O `uv run` usa o ambiente virtual do projeto automaticamente. Se preferir ativar o ambiente manualmente:

```bash
# Windows (PowerShell)
.venv\Scripts\Activate.ps1

# Linux / Mac
source .venv/bin/activate

flask run
```

O servidor sobe em `http://127.0.0.1:5000`. Para parar, use `Ctrl + C`.

## Como acessar a rota inicial

Abra `http://127.0.0.1:5000/` no navegador ou use o terminal:

```bash
curl -i http://localhost:5000/
```

No PowerShell, use `curl.exe` em vez de `curl`.

Resposta esperada:

- **Status:** `200 OK`
- **Content-Type:** `application/json`
- **Corpo:**

```json
{"message": "API de chamados em funcionamento"}
```