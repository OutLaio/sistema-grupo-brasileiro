# 📊 Sistema de Gerenciamento de Solicitações de Marketing - Rota Transportes - Frontend

Este é o frontend do sistema de gerenciamento de solicitações de marketing desenvolvido para o Grupo Rota Transportes e Grupo Brasileiro. A aplicação é baseada em Angular e tem como objetivo facilitar o acompanhamento e gestão de projetos de marketing, integrando clientes, colaboradores e supervisores.

<br>

## 📝 Licença

Este projeto é privado e de uso exclusivo do Grupo Rota Transportes e Grupo Brasileiro.

<br>

## 🤝 Colaboradores

- Desenvolvedores Frontend: Darley Souza Sampaio e Laio Rodrigues
- UI/UX Designer: Darley Souza Sampaio e Laio Rodrigues
- Scrum Master: Laio Rodrigues
- Gestor de Projeto: Marcelo Silva
- Empresa: Rota Transportes e Grupo Brasileiro

<br>

## 📁 Estrutura do Projeto

O projeto é dividido em dois repositórios:
- **Frontend** (este repositório): Interface do usuário em Angular
- **Backend**: API RESTful que fornece os dados e autenticação em Spring

<br>

## 🚀 Funcionalidades

### 🔐 Sistema de Autenticação
- Login de usuários (colaboradores, supervisores e clientes)
- Cadastro de **colaboradores** realizado exclusivamente por **supervisores**
- Cadastro de **clientes** via link com **tempo de expiração**
- Solicitação de recuperação de senha
- Alteração de senha

### 🏠 Página Principal - Quadro Kanban
Visualização de projetos distribuídos nas seguintes etapas:
- A Fazer (Solicitações recém feitas)
- Em Andamento (Solicitações aprovadas e colaborador alocado)
- Aguardando Aprovação (Aguardando aprovação das artes pelas partes)
- Aprovado (Aprovado e aguardando confecção ou entrega)
- Em Confecção (Projeto físico em cofecção)
- Concluído (Projeto concluído e entregue)
- Standby (Projeto interrompido)

Cada card representa uma solicitação de projeto com:
- Tipo do projeto
- Colaborador responsável
- Nome do projeto
- Cliente
- Data de solicitação

Clicar no card leva para a **página de detalhes** da solicitação.


### 📝 Cadastro de Solicitação
- Sistema de formulários dinâmicos com base no tipo de projeto
- Campos dinâmicos conforme o tipo de briefing selecionado
- Formulário muda a depender das opções selecionadas pelo usuário
- Três tipos de briefings atualmente (mais serão adicionados futuramente)

### 📄 Página de Informações da Solicitação
- Visualização completa das informações do projeto
- Atribuição de data de entrega e status (por colaborador ou supervisor)
- Sistema de **mensagens tipo chat** entre colaborador e cliente
  - Supervisor também pode visualizar e interagir
- Mensagens automáticas apareceram no chat de acordo com o avançar do projeto
- Upload e aprovação de artes criadas pelo colaborador
  - Após aprovação, é possível enviar para confecção (quando aplicável)

### 👨‍💼 Gestão de Usuários
- Cadastro e visualização de **colaboradores**
- Visualização de **clientes**
- Geração de link para cadastro de cliente com expiração

### 👤 Página de Perfil
- Visualização e edição dos dados do usuário:
  - Nome
  - Telefone
  - Função
  - Setor/Departamento
  - Núcleo operacional/Agência
  - Avatar
- O campo **email** não pode ser editado

<br>

## 🛠️ Principais Tecnologias Utilizadas

- **Angular 18** – Framework principal para construção da SPA
- **Angular Material** – Componentes UI modernos e responsivos
- **Bootstrap 5** – Estilização e grid layout
- **Ngx-Drag-Drop** – Sistema de arrastar e soltar no Kanban
- **Ngx-Scrollbar** – Scroll customizado responsivo
- **Ngx-Toastr** – Notificações toast amigáveis
- **Ngx-Mask** – Máscaras para campos de entrada
- **SweetAlert2** – Alertas modernos e customizáveis
- **Compodoc** – Documentação completa do projeto
- **RxJS** – Programação reativa para manipulação de dados
- **TypeScript** – Linguagem principal baseada em JavaScript

<br>

## 🐳 Deploy

O projeto está configurado para **deploy em ambiente AWS**, utilizando **Docker**.
