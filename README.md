<div align="center">

<img src="readme_roxo_animado.gif" width="100%">

# 🗳️ sistema de gerenciamento eleitoral

### `php` • `mysql` • `crud` • `pdo`

<img src="https://img.shields.io/badge/PHP-9b7ede?style=for-the-badge&logo=php&logoColor=white">
<img src="https://img.shields.io/badge/MySQL-b89ae6?style=for-the-badge&logo=mysql&logoColor=white">
<img src="https://img.shields.io/badge/CRUD-c8b6e8?style=for-the-badge">
<img src="https://img.shields.io/badge/SCRUM-a78bca?style=for-the-badge">

<br><br>

<a href="#-sobre-o-projeto">✨ sobre</a> •
<a href="#-funcionalidades">⚙️ funcionalidades</a> •
<a href="#-estrutura-do-projeto">📁 estrutura</a> •
<a href="#-tecnologias">💻 tecnologias</a> •
<a href="#-como-executar">🚀 executar</a>

</div>

---

## 💜 sobre o projeto

o **sistema de gerenciamento eleitoral** foi desenvolvido para a atividade **SAEP – desenvolvimento de CRUD em PHP**, realizada na escola senai a. jacob lafer.

o objetivo do projeto é criar uma aplicação web para o gerenciamento de informações de **eleitores e candidatos**, permitindo realizar as principais operações de um CRUD:

```text
create  →  cadastrar
read    →  consultar
update  →  atualizar
delete  →  excluir
```

a aplicação utiliza **PHP** para o processamento das informações e **MySQL** para armazenamento e gerenciamento dos dados.

a comunicação entre a aplicação e o banco de dados é realizada utilizando **PDO** e **Prepared Statements**.

---

## ✨ funcionalidades

<details>
<summary>👤 <b>eleitores</b> — clique para visualizar</summary>

<br>

- ➕ cadastro de eleitores
- 🔎 consulta de eleitores
- ✏️ atualização de informações
- 🗑️ exclusão de eleitores
- 🔗 associação com candidato

</details>

<br>

<details>
<summary>🗳️ <b>candidatos</b> — clique para visualizar</summary>

<br>

- ➕ cadastro de candidatos
- 🔎 consulta de candidatos
- ✏️ atualização de informações
- 🗑️ exclusão de candidatos
- 🏛️ gerenciamento de partido e número

</details>

<br>

<details>
<summary>🔐 <b>segurança e banco de dados</b> — clique para visualizar</summary>

<br>

- 🔗 chave estrangeira entre as tabelas
- 🔑 chaves primárias
- 🚫 restrições de unicidade
- 🛡️ PDO
- 🔒 Prepared Statements
- 🗄️ MySQL

</details>

---

## 📁 estrutura do projeto

a estrutura do repositório está organizada da seguinte maneira:

```text
📦 sistema-eleitoral
│
├── 📄 .gitattributes
│
├── 🗑️ candidato_excluir.php
├── 📝 candidato_form.php
├── 👥 candidatos.php
│
├── ⚙️ config.php
├── 🗄️ database.sql
│
├── 🗑️ eleitor_excluir.php
├── 📝 eleitor_form.php
├── 👤 eleitores.php
│
├── 🏠 index.php
│
└── 📖 README.md
```

### 🔍 entendendo os arquivos

<details>
<summary>🗳️ <b>arquivos de candidatos</b></summary>

<br>

| arquivo | função |
|---|---|
| `candidatos.php` | gerenciamento e visualização dos candidatos |
| `candidato_form.php` | formulário para cadastro e edição |
| `candidato_excluir.php` | exclusão de candidatos |

</details>

<br>

<details>
<summary>👤 <b>arquivos de eleitores</b></summary>

<br>

| arquivo | função |
|---|---|
| `eleitores.php` | gerenciamento e visualização dos eleitores |
| `eleitor_form.php` | formulário para cadastro e edição |
| `eleitor_excluir.php` | exclusão de eleitores |

</details>

<br>

<details>
<summary>⚙️ <b>arquivos de configuração</b></summary>

<br>

| arquivo | função |
|---|---|
| `config.php` | configuração da conexão utilizada pelo sistema |
| `database.sql` | estrutura do banco de dados |
| `index.php` | página inicial da aplicação |
| `.gitattributes` | configurações do git |

</details>

---

## 💻 tecnologias

<div align="center">

| tecnologia | utilizada para |
|:---:|---|
| 🐘 **PHP** | processamento e lógica da aplicação |
| 🐬 **MySQL** | armazenamento dos dados |
| 🔗 **PDO** | comunicação com o banco |
| 🔐 **Prepared Statements** | consultas mais seguras |
| 🔄 **CRUD** | gerenciamento dos registros |
| 📋 **SCRUM** | organização do desenvolvimento |

</div>

---

## 🔄 funcionamento

```text
                         🗳️ SISTEMA ELEITORAL
                                  │
                 ┌────────────────┴────────────────┐
                 │                                 │
              👤 ELEITOR                        🗳️ CANDIDATO
                 │                                 │
        ┌────────┼────────┐              ┌─────────┼────────┐
        ↓        ↓        ↓              ↓         ↓        ↓
       ➕       🔎       ✏️              ➕        🔎       ✏️
     criar    consultar  editar        criar    consultar  editar
        │        │        │              │         │        │
        └────────┴────────┘              └─────────┴────────┘
                 │                                 │
                 ↓                                 ↓
                🗑️                               🗑️
              excluir                           excluir
```

---

## 🗄️ banco de dados

o banco de dados possui duas entidades principais:

```text
╭──────────────────────────╮
│       🗳️ CANDIDATO       │
├──────────────────────────┤
│ nome                     │
│ número                   │
│ partido                  │
╰────────────┬─────────────╯
             │
             │ 🔗 relacionamento
             ↓
╭──────────────────────────╮
│        👤 ELEITOR        │
├──────────────────────────┤
│ nome                     │
│ cpf                      │
│ título de eleitor        │
│ candidato associado      │
╰──────────────────────────╯
```

o relacionamento entre as tabelas é realizado por meio de uma **chave estrangeira**, contribuindo para a integridade dos dados.

---

## 🛡️ segurança

o projeto utiliza **PDO** e **Prepared Statements** na comunicação com o banco de dados.

```text
          🔐 SEGURANÇA
               │
        ┌──────┴──────┐
        ↓             ↓
       PDO      PREPARED STATEMENTS
        │             │
        └──────┬──────┘
               ↓
       🛡️ CONSULTAS MAIS SEGURAS
```

também foram utilizadas chaves primárias, chaves estrangeiras e restrições de unicidade.

---

## 📸 estrutura real do repositório

<div align="center">

<img src="estrutura-projeto.png" width="700">

<br>

<i>arquivos presentes no projeto</i>

</div>

---

## 🚀 como executar

<details>
<summary>1️⃣ 💻 <b>requisitos</b></summary>

<br>

para executar o projeto localmente, utilize um ambiente com:

- PHP
- MySQL
- Apache
- XAMPP, WAMP ou equivalente

</details>

<br>

<details>
<summary>2️⃣ 🗄️ <b>configurar o banco</b></summary>

<br>

importe o arquivo:

```text
database.sql
```

no MySQL.

</details>

<br>

<details>
<summary>3️⃣ ⚙️ <b>configurar a conexão</b></summary>

<br>

verifique as configurações de conexão no arquivo:

```text
config.php
```

</details>

<br>

<details>
<summary>4️⃣ 🌐 <b>abrir o sistema</b></summary>

<br>

coloque o projeto na pasta do servidor local e acesse:

```text
http://localhost/nome-do-projeto/
```

</details>

---

## 📋 metodologia scrum

o desenvolvimento foi organizado utilizando a metodologia ágil **SCRUM**.

a equipe foi dividida em diferentes responsabilidades:

- 👑 Product Owner
- 🔄 Scrum Master
- 💻 Desenvolvimento
- 🗄️ Banco de Dados
- 🧪 Qualidade
- 📝 Documentação
- 🎨 Design

a utilização do scrum auxiliou na organização das atividades e no acompanhamento da sprint.

---

## 🧪 testes

| funcionalidade | status |
|:---|:---:|
| ➕ cadastro | ✅ |
| 🔎 consulta | ✅ |
| ✏️ atualização | ✅ |
| 🗑️ exclusão | ✅ |
| 🔗 relacionamento entre tabelas | ✅ |
| 🔐 validação e segurança | ✅ |
| 🌐 redirecionamento das páginas | ✅ |

---

## 📚 projeto acadêmico

<details>
<summary>📖 <b>informações</b></summary>

<br>

**instituição:** escola senai a. jacob lafer

**atividade:** SAEP – desenvolvimento de CRUD em PHP

**curso:** desenvolvimento de sistemas

**período:** 2º semestre de 2026

</details>

---

## 👥 equipe

<div align="center">

andressa papini • bruno tognoli • gabrilly roseghini •  
guilherme gandini • gustavo santana • henrique del rey •  
isaque ruas • josé augusto • julia pacheco •  
**larissa eduarda** • quezia brito • rafaela merloto

</div>

---

<div align="center">

## 💜 desenvolvido com código + criatividade + trabalho em equipe

<img src="https://img.shields.io/badge/SAEP-2026-c8b6e8?style=for-the-badge">
<img src="https://img.shields.io/badge/SENAI-A._JACOB._LAFER-a78bca?style=for-the-badge">

<br><br>

**⭐ gostou do projeto? deixe uma estrela!**

</div>
