---

# 📁 Projeto Integrador - Sistema de Cadastro: **Last Seven**

Este repositório contém o código-fonte e a estrutura do projeto **Last Seven**, um site desenvolvido como parte do **Projeto Integrador** do curso técnico em Informática (SENAC - Porto Velho, RO). O sistema tem como objetivo o **cadastro de usuários e o gerenciamento de contatos de clientes** que solicitam serviços de programação.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5** – Estruturação das páginas web
* **CSS3** – Estilização e responsividade
* **JavaScript** – Validações e interações na interface
* **PHP** – Backend e integração com banco de dados
* **MySQL** – Banco de dados relacional
* **Java (Swing + JDBC)** – Aplicação desktop para leitura e gerenciamento dos cadastros

---

## 💡 Funcionalidades

### 🌐 Site Web

* Página Home com apresentação da empresa
* Página de Equipe, Projetos e Contato
* Formulário de contato com envio de dados para o banco de dados
* Validação de campos com JavaScript

### ⚙️ Backend (PHP)

* Processamento de dados do formulário
* Conexão segura com banco de dados usando PDO
* Inserção dos cadastros no MySQL

### 🖥️ Aplicação Desktop (Java)

* Consulta ao banco de dados via JDBC
* Listagem de cadastros realizados
* Atualização e gerenciamento do status dos cadastros

---

## 🧱 Estrutura de Diretórios (MVC)

```bash
/
├── index.html                  # Página inicial (View principal)
├── imagens/                    # Logos e imagens utilizadas no site
│   ├── Logo.jpg
│   ├── Insta.jpg
│   ├── facebook.jpg
│   └── Linkdin.jpg
├── abas/                       # Páginas internas (Views secundárias)
│   ├── equipes/equipe.html
│   ├── projetos/projetos.html
│   └── pedidos/contato.html
├── src/                        # Códigos de estilo e scripts (Controller web)
│   └── estilo_index.css
├── Desktop/                    # Aplicação Java para gerenciamento (Controller desktop)
│   └── AplicativoDesktop.java
├── php/                        # Arquivos de backend PHP (Controller do servidor)
│   ├── conectar.php
│   └── processar_formulario.php
├── sql/                        # Script de banco de dados (Model)
│   └── lastseven_db.sql
└── README.md                   # Documentação do projeto
```

### 🧭 Organização segundo o modelo **MVC**:

* **Model (Modelo):** Banco de dados MySQL e scripts `.sql` para estrutura da tabela de cadastros.
* **View (Visão):** Arquivos `.html` dentro da raiz e da pasta `abas/` representam as interfaces que o usuário acessa.
* **Controller (Controle):**

  * **Web:** Scripts CSS/JS em `src/` e os arquivos PHP responsáveis pela lógica de envio dos dados.
  * **Desktop:** Aplicativo Java que se conecta ao banco para consultar e atualizar dados.

---

## 📂 Banco de Dados

* **Nome:** `lastseven_db`
* **Tabela:** `cadastros`
* **Campos:** `id`, `nome`, `email`, `servico`, `mensagem`, `status`, `data_envio`
* O script de criação está na pasta `/sql/`.

---

## ▶️ Como Executar o Projeto

1. Clone este repositório:

   ```bash
   git clone https://github.com/seuusuario/last-seven.git
   ```

2. Importe o banco de dados MySQL com o arquivo `lastseven_db.sql`.

3. Configure os dados de conexão em `php/conectar.php`.

4. Inicie um servidor local (como XAMPP ou WAMP) e acesse `index.html` via navegador.

5. Para executar o aplicativo Java:

   * Compile e execute `AplicativoDesktop.java`
   * Certifique-se de que o banco de dados esteja ativo e com as credenciais corretas.

---

## 👥 Equipe

* **Adaiana Duarte** – Scrum Master / Planejamento
* **Vinícius Moreira** – Front-End & Back-End
* **Eduarda Pinheiro** – Validação & Testes
* **Kléber Lucas** – Banco de Dados
* **Gean Greguy** – Banco de Dados
* **Nicholas Bollate** – Documentação
* **João Silva** – Documentação

---

## 📜 Licença

Este projeto é apenas para fins **educacionais** e não possui fins **comerciais**.

---
