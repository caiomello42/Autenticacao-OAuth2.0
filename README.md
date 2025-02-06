# 🌐 Conectando Aplicações com OAuth 2.0 e GitHub 🚀

Este projeto tem como objetivo a integração de OAuth 2.0 em uma aplicação Django, usando o GitHub como provedor de autenticação. A ideia é simplificar o processo de login e aumentar a segurança das aplicações, permitindo que os usuários façam login sem precisar expor suas credenciais.

## 🛠️ Como Funciona?

OAuth 2.0 é um protocolo de autorização que permite que aplicações acessem informações do usuário em nome dele, sem que suas credenciais sejam expostas.

### 1️⃣ Registro da Aplicação no GitHub

Antes de começar a implementação, a aplicação foi registrada nas configurações do GitHub Developer, gerando um **Client ID** e um **Client Secret** necessários para configurar o fluxo de autenticação.

### 2️⃣ Fluxo de Autenticação

A integração com o GitHub segue os seguintes passos:

1. O usuário clica no botão **"Login com GitHub"** na aplicação.
2. O usuário autoriza o acesso aos dados da sua conta do GitHub.
3. A aplicação é redirecionada para uma URL de **callback**, onde um código temporário é recebido.
4. O código é trocado por um **Access Token** que permite à aplicação acessar os dados do usuário.

### 3️⃣ Cadastro Automático no Django Admin

Uma funcionalidade adicional implementada foi o **registro automático** de usuários que fazem login via GitHub. Com isso, sempre que um usuário se autentica pela primeira vez, ele é automaticamente registrado no banco de dados e pode ser visualizado e gerido diretamente na interface administrativa do Django.

## 🔒 Benefícios da Integração

- **Segurança:** A integração reduz a responsabilidade de armazenar senhas de usuários, delegando essa função ao GitHub.
- **Facilidade:** Usuários podem utilizar suas credenciais do GitHub para autenticação, sem a necessidade de criar novas senhas.
- **Monitoramento:** O registro automático no Django Admin facilita a gestão dos usuários e o controle de permissões dentro do sistema.

## 📋 Tecnologias Utilizadas

- Python
- Django
- OAuth 2.0
- GitHub (como provedor de autenticação)

