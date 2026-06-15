# Projeto: Agenda de Contatos (CRUD)

Este projeto consiste em uma aplicação web simples para gerenciamento de contatos, permitindo a criação, leitura, atualização, busca e exclusão (CRUD) de registros. A aplicação consome um backend como serviço (BaaS) para persistência de dados em tempo real.

## 👥 Integrantes do Grupo

- **Nome do Integrante** - Hyago Fernando Ferreira Rodrigues

---

## 🗄️ Banco de Dados Escolhido

Para este projeto, foi utilizado o **Supabase**.

**Especificações:**

- **Tecnologia:** PostgreSQL (Gerenciado).
- **Interface:** RESTful API via Supabase JS SDK.
- **Tabela:** `contato`
- **SQL da Tabela:**
```
CREATE TABLE CONTATO (
    ID  SERIAL PRIMARY KEY,
    EMAIL VARCHAR(255),
    NOME  VARCHAR(255),
    TELEFONE VARCHAR(25),
    OBS    VARCHAR(255),
    DTCONTATO  DATE 
);
```
---

## 🚀 Tecnologias Utilizadas

- **Frontend:** HTML5, CSS3 (Estilos Inline) e JavaScript (Vanilla).
- **Backend & DB:** Supabase (PostgreSQL).
- **CDN:** [Supabase SDK v2](https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2).

---

## ⚙️ Configuração do Projeto

Para que a aplicação funcione corretamente com o banco de dados, os seguintes passos foram realizados:

1.  Criação de um projeto no painel do [Supabase](https://app.supabase.com/).
2.  Criação da tabela `contato` no SQL Editor ou Table Editor.
3.  Configuração das chaves de acesso no arquivo `index.html`:
    - `SUPABASE_URL`: URL do projeto.
    - `SUPABASE_KEY`: Chave anônima (anon key) para acesso público.

---

## 🛠️ Funcionalidades

1.  **Inserir:** Cadastro de novos contatos com validação de campos obrigatórios.
2.  **Listar:** Exibição dinâmica dos contatos recuperados do banco de dados.
3.  **Editar:** Atualização de dados de contatos existentes.
4.  **Excluir:** Remoção definitiva de contatos da base de dados.
5.  **Buscar:** Filtragem de contatos por nome utilizando a cláusula `ilike` do PostgreSQL.
