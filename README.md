# FAST-API Project

Este projeto é uma API de perguntas e respostas (quiz) construída com FastAPI, SQLAlchemy e PostgreSQL.

## Como baixar o projeto

Clone o repositório usando o comando abaixo no terminal (PowerShell ou terminal do VS Code):

```sh
git clone https://github.com/Marcos-Correa-dev/FAST-API-project
cd FAST-API-project
```

## Como criar e ativar o ambiente virtual

No PowerShell, execute:

```sh
python -m venv env
.\env\Scripts\Activate
```

Se estiver usando o terminal do VS Code, basta rodar os mesmos comandos acima.

## Como instalar as dependências

Com o ambiente virtual ativado, instale as dependências:

```sh
pip install fastapi[all] sqlalchemy psycopg2
```

## Como rodar a aplicação

Execute o comando abaixo no terminal:

```sh
uvicorn main:app --reload
```

A aplicação estará disponível em: [http://127.0.0.1:8000](http://127.0.0.1:8000)

## Como usar o Swagger

Acesse a documentação interativa do Swagger em:

[http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

Você pode testar os endpoints diretamente por essa interface.

## Como verificar os dados no banco PostgreSQL usando DataGrip

1. Abra o DataGrip.
2. Clique em **+** para adicionar uma nova conexão.
3. Escolha **PostgreSQL**.
4. Preencha os dados de conexão conforme o arquivo `database.py`:
   - Host: `localhost`
   - Porta: `5432`
   - Usuário: `postgres`
   - Senha: `admin@1212` ou `postegres ` ou `senha no qual você criopu` 
   - Banco de dados: `quizapplication`
5. Clique em **Test Connection** e depois em **OK**.

Agora você pode visualizar e manipular as tabelas `questions` e `choices` diretamente pelo DataGrip.

---

**Dica:** Sempre ative o ambiente virtual antes de rodar comandos Python ou instalar
