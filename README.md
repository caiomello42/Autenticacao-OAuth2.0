# 🌐 **Conectando Aplicações com OAuth 2.0 e GitHub** 🚀

Este projeto tem como objetivo integrar o **OAuth 2.0** em uma aplicação Django, utilizando o **GitHub** como provedor de autenticação. A ideia é simplificar o processo de login e aumentar a segurança das aplicações, permitindo que os usuários façam login sem a necessidade de expor suas credenciais.

---

## 🛠️ **Como Funciona?**

OAuth 2.0 é um protocolo de autorização que permite que as aplicações acessem informações do usuário em seu nome, sem que as credenciais sejam expostas. 

### 1️⃣ **Registro da Aplicação no GitHub**

Antes de iniciar a implementação, a aplicação foi registrada no [GitHub Developer Settings](https://github.com/settings/developers), gerando um **Client ID** e um **Client Secret**, que são necessários para configurar o fluxo de autenticação.

### 2️⃣ **Fluxo de Autenticação**

A integração com o GitHub segue os seguintes passos:

1. O usuário clica no botão **"Login com GitHub"** na aplicação.
2. O usuário autoriza o acesso aos dados da sua conta do GitHub.
3. A aplicação é redirecionada para uma URL de **callback**, onde um código temporário é recebido.
4. O código é trocado por um **Access Token**, que permite à aplicação acessar os dados do usuário.

### 3️⃣ **Cadastro Automático no Django Admin**

Uma funcionalidade adicional implementada foi o **registro automático** de usuários que se autenticam via GitHub. Sempre que um usuário se autentica pela primeira vez, ele é automaticamente registrado no banco de dados, e seu perfil pode ser visualizado e gerido diretamente na interface administrativa do Django.

---

## 🔒 **Benefícios da Integração**

- **Segurança:** A integração elimina a necessidade de armazenar senhas dos usuários, delegando essa responsabilidade ao GitHub.
- **Facilidade:** Usuários podem fazer login utilizando suas credenciais do GitHub, sem precisar criar novas senhas.
- **Gestão Simplificada:** O registro automático no Django Admin facilita a gestão de usuários e o controle de permissões dentro do sistema.
- **Escalabilidade:** A integração com OAuth 2.0 permite uma fácil expansão para outros provedores de autenticação no futuro.

---

## 📋 **Tecnologias Utilizadas**

- **Python**: Linguagem de programação backend.
- **Django**: Framework web para desenvolvimento de aplicações rápidas e seguras.
- **OAuth 2.0**: Protocolo de autorização para autenticação segura.
- **GitHub**: Provedor de autenticação utilizado para login.
  
---

## 🚀 **Como Rodar o Projeto**

1. Clone o repositório:
   ```bash
   git clone https://github.com/caiomello42/Autenticacao-OAuth2.0.git
