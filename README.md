# 🗳️ sistema de gerenciamento eleitoral

<div align="center">

### 💻 CRUD • PHP • MYSQL • PDO

**sistema web desenvolvido para gerenciamento de eleitores e candidatos**

[📌 sobre o projeto](#-sobre-o-projeto) •
[⚙️ funcionalidades](#️-funcionalidades) •
[🗂️ estrutura](#️-estrutura-do-projeto) •
[🚀 como executar](#-como-executar) •
[👥 equipe](#-equipe)

</div>

---

## ✨ sobre o projeto

o **sistema de gerenciamento eleitoral** foi desenvolvido como atividade do **SAEP – desenvolvimento de sistemas**, com o objetivo de aplicar na prática conhecimentos de **desenvolvimento web, banco de dados, segurança e gestão ágil de projetos**.

a aplicação permite realizar o gerenciamento de informações relacionadas a **eleitores e candidatos**, utilizando o conceito de **CRUD**:

> 🟢 **create** → cadastrar  
> 🔵 **read** → consultar  
> 🟡 **update** → atualizar  
> 🔴 **delete** → excluir

o projeto foi desenvolvido utilizando **php + mysql**, com comunicação através do **pdo** e utilização de **prepared statements**, contribuindo para uma aplicação mais organizada e segura. :contentReference[oaicite:1]{index=1}

---

## 🎯 objetivo

desenvolver uma aplicação web capaz de organizar e gerenciar dados eleitorais de maneira estruturada, permitindo o cadastro, consulta, edição e exclusão de registros de **eleitores e candidatos**.

o banco de dados possui duas entidades principais:

- 👤 **eleitores**
- 🗳️ **candidatos**

os registros possuem relacionamentos e restrições para manter a integridade das informações armazenadas. :contentReference[oaicite:2]{index=2}

---

## ⚙️ funcionalidades

### 👤 gerenciamento de eleitores

- ➕ cadastrar eleitor
- 🔎 consultar eleitores
- ✏️ editar informações
- 🗑️ excluir eleitor
- 🔗 associar eleitor a um candidato

### 🗳️ gerenciamento de candidatos

- ➕ cadastrar candidato
- 🔎 consultar candidatos
- ✏️ editar informações
- 🗑️ excluir candidato

### 🔐 segurança e banco de dados

- conexão utilizando **pdo**
- utilização de **prepared statements**
- prevenção contra riscos de **sql injection**
- utilização de **chaves primárias**
- utilização de **chaves estrangeiras**
- restrições de **unicidade**
- relacionamento entre eleitores e candidatos

essas práticas foram utilizadas para melhorar a organização, segurança e integridade dos dados. :contentReference[oaicite:3]{index=3}

---

## 🛠️ tecnologias utilizadas

<div align="center">

| tecnologia | utilização |
|---|---|
| 🐘 **php** | lógica e processamento da aplicação |
| 🐬 **mysql** | armazenamento e gerenciamento dos dados |
| 🔗 **pdo** | comunicação entre php e banco de dados |
| 🔐 **prepared statements** | segurança nas consultas |
| 🔄 **crud** | gerenciamento dos registros |
| 📋 **scrum** | organização do desenvolvimento |

</div>

---

## 🗂️ estrutura do projeto

```text
📁 sistema-eleitoral
│
├── 📄 .gitattributes
│
├── 📄 candidato_excluir.php
├── 📄 candidato_form.php
├── 📄 candidatos.php
│
├── 📄 config.php
├── 📄 database.sql
│
├── 📄 eleitor_excluir.php
├── 📄 eleitor_form.php
├── 📄 eleitores.php
│
└── 📄 index.php
