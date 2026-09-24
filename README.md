<div align="center">

#  🖥️ sistema de gerenciamento eleitoral

### ✦ CRUD • PHP • MYSQL • PDO ✦

<img src="https://img.shields.io/badge/PHP-9b7ede?style=for-the-badge&logo=php&logoColor=white">
<img src="https://img.shields.io/badge/MySQL-b89ae6?style=for-the-badge&logo=mysql&logoColor=white">
<img src="https://img.shields.io/badge/CRUD-c8b6e8?style=for-the-badge">
<img src="https://img.shields.io/badge/SCRUM-a78bca?style=for-the-badge">

<br><br>

>  um sistema web desenvolvido para o gerenciamento de  
> **eleitores e candidatos**, utilizando php e mysql.

<br>

<a href="#-sobre-o-projeto">
<img src="https://img.shields.io/badge/✨_sobre_o_projeto-c8b6e8?style=for-the-badge">
</a>

<a href="#-funcionalidades">
<img src="https://img.shields.io/badge/⚙️_funcionalidades-b89ae6?style=for-the-badge">
</a>

<a href="#-estrutura">
<img src="https://img.shields.io/badge/📁_estrutura-d8c7ed?style=for-the-badge">
</a>

<a href="#-como-executar">
<img src="https://img.shields.io/badge/🚀_executar-a78bca?style=for-the-badge">
</a>

</div>

---

## 💜 sobre o projeto

<details>
<summary><b>✨ clique aqui para conhecer o projeto</b></summary>

<br>

o **sistema de gerenciamento eleitoral** foi desenvolvido como atividade do **saep – desenvolvimento de sistemas**, com o objetivo de aplicar conhecimentos de desenvolvimento web, banco de dados, segurança e gestão ágil.

a aplicação permite o gerenciamento de informações relacionadas a:

- 👤 eleitores
- 🗳️ candidatos
- 🔗 relacionamento entre registros
- 🗄️ banco de dados

o sistema utiliza o conceito de **crud**:

| ação | significado |
|---|---|
| 🟣 create | cadastrar |
| 🔵 read | consultar |
| 🟡 update | atualizar |
| 🔴 delete | excluir |

</details>

---

## ✨ tecnologias

<div align="center">

| 💜 tecnologia | 🎯 utilização |
|:---:|---|
| 🐘 **php** | processamento da aplicação |
| 🐬 **mysql** | armazenamento dos dados |
| 🔗 **pdo** | comunicação com o banco |
| 🔐 **prepared statements** | segurança |
| 🔄 **crud** | gerenciamento dos registros |
| 📋 **scrum** | organização da equipe |

</div>

---

## ⚙️ funcionalidades

<details>
<summary>👤 <b>gerenciamento de eleitores</b></summary>

<br>

➕ cadastro de eleitor  
🔎 consulta de eleitor  
✏️ edição de informações  
🗑️ exclusão de eleitor  
🔗 associação com candidato  

</details>

<br>

<details>
<summary>🗳️ <b>gerenciamento de candidatos</b></summary>

<br>

➕ cadastro de candidato  
🔎 consulta de candidato  
✏️ edição de informações  
🗑️ exclusão de candidato  

</details>

<br>

<details>
<summary>🔐 <b>segurança</b></summary>

<br>

o projeto utiliza:

- pdo
- prepared statements
- chaves primárias
- chaves estrangeiras
- restrições de unicidade

essas práticas foram utilizadas para melhorar a segurança e a integridade dos dados.

</details>

---

## 📁 estrutura

<div align="center">

### 🗂️ arquivos do projeto

</div>

```text
💜 sistema-eleitoral
│
├── 📄 .gitattributes
│
├── 🗳️ candidato_excluir.php
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
└── 🏠 index.php
