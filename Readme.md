# 🚀 Desafio de Desenvolvimento: Sistema de Tarefas!

## Objetivo do Desafio
O objetivo deste desafio é desenvolver um sistema simples de gerenciamento de tarefas. Você pode escolher fazer apenas o **front-end**, o **back-end**, ou ambos para criar um projeto **full-stack**. Esse desafio é ideal para quem está começando e quer praticar as habilidades de programação.

## O que é um Sistema de Tarefas?
É uma aplicação onde o usuário pode:
- Adicionar uma nova tarefa.
- Visualizar todas as tarefas criadas.
- Editar as tarefas existentes.
- Excluir tarefas.
- Alterar o status de uma tarefa (completa ou não completa).

## Como Participar
1. **Escolha o tipo de desafio**:
   - **Front-end**: Criação da interface do usuário.
   - **Back-end**: Desenvolvimento da API e conexão com o banco de dados.
   - **Full-stack**: Fazer tanto o front-end quanto o back-end e integrá-los.

2. **Escolha a tecnologia que deseja usar**:
   - **Front-end**:
     - HTML + CSS (você pode usar frameworks como Bootstrap, TailwindCSS, etc.)
     - JavaScript puro ou usando frameworks como React, Vue.js ou Angular.
   - **Back-end**:
     - Node.js (JavaScript ou TypeScript)
     - Java (Spring Boot)
     - Python (Flask)
     - PHP (Laravel)
     - Ou qualquer uma dessas linguagens sem framework.

## 🔧 O que Deve Ser Feito no **Front-end**?
A interface do sistema de tarefas deve permitir ao usuário:
1. **Adicionar nova tarefa**:
   - Criar um formulário com campos:
     - Título da tarefa.
     - Descrição da tarefa.
   - Quando o usuário clicar no botão "Adicionar", a nova tarefa deve aparecer na lista de tarefas.

2. **Visualizar todas as tarefas**:
   - Exibir uma lista de todas as tarefas criadas, incluindo:
     - Título.
     - Descrição.
     - Status (se a tarefa está completa ou não).

3. **Editar uma tarefa existente**:
   - Adicionar uma opção de editar uma tarefa já criada.
   - Criar um formulário que permite ao usuário alterar o título, descrição e status da tarefa.

4. **Excluir uma tarefa**:
   - Adicionar um botão de "Excluir" ao lado de cada tarefa na lista.
   - Quando o botão for clicado, a tarefa deve ser removida da lista.

5. **Alterar o status da tarefa**:
   - Adicionar uma forma de marcar a tarefa como completa ou não completa (por exemplo, um checkbox ou um botão de "Concluir").

## Estrutura básica da interface:
- Use HTML e CSS para criar uma interface simples, ou escolha frameworks como **Bootstrap** ou **TailwindCSS** para estilizar.
- Para a parte interativa (adicionar, editar, excluir), você pode usar **JavaScript** ou uma biblioteca/framework como **React**, **Vue.js**, ou **Angular**.

## 🔧 O que Deve Ser Feito no **Back-end**?
Se você optar por desenvolver o back-end, aqui está uma lista de funcionalidades que você deve implementar:

1. **API para Gerenciamento de Tarefas**:
   - Criar uma API REST com os seguintes endpoints:
     - `POST /tarefas`: Para adicionar uma nova tarefa.
     - `GET /tarefas`: Para listar todas as tarefas.
     - `PUT /tarefas/:id`: Para atualizar uma tarefa (editar título, descrição ou status).
     - `DELETE /tarefas/:id`: Para excluir uma tarefa.

2. **Banco de Dados**:
   - Use um banco de dados para armazenar as tarefas (pode ser MySQL, PostgreSQL, MongoDB ou outro de sua escolha).
   - Estrutura do banco de dados:
     - Cada tarefa deve ter um **ID** (gerado automaticamente).
     - **Título** (texto).
     - **Descrição** (texto).
     - **Status** (booleano: completa ou não completa).

3. **Estrutura de Dados da Tarefa**:
   - Cada tarefa deve conter os seguintes campos:
     - `id`: identificador único da tarefa.
     - `titulo`: o título da tarefa.
     - `descricao`: a descrição da tarefa.
     - `status`: um valor booleano (verdadeiro/falso) para indicar se a tarefa está completa ou não.

4. **Rotas da API**:
   - `POST /tarefas`: para criar uma nova tarefa.
     - A API deve esperar um corpo JSON com `titulo` e `descricao`.
   - `GET /tarefas`: para listar todas as tarefas.
   - `PUT /tarefas/:id`: para editar uma tarefa existente.
     - A API deve esperar um corpo JSON com `titulo`, `descricao`, e `status`.
   - `DELETE /tarefas/:id`: para deletar uma tarefa existente.

## 🔄 O que Deve Ser Feito no **Full-stack**?
Se você quiser fazer o desafio completo (front-end + back-end), aqui está o que deve ser feito:

1. **Integração Front-end e Back-end**:
   - O front-end deve se comunicar com o back-end através das chamadas à API.
   - Quando o usuário adicionar, editar ou excluir uma tarefa na interface, as mudanças devem ser refletidas no banco de dados via API.

2. **Chamadas à API**:
   - Use **fetch** ou **Axios** no front-end para fazer requisições HTTP aos endpoints da API que você criou no back-end.
   - Exemplos:
     - Para adicionar uma tarefa: `POST /tarefas`.
     - Para listar todas as tarefas: `GET /tarefas`.
     - Para editar uma tarefa: `PUT /tarefas/:id`.
     - Para excluir uma tarefa: `DELETE /tarefas/:id`.

## 📋 Regras do Desafio
- O código deve ser bem organizado e fácil de entender.
- Use boas práticas de programação (nomes de variáveis claros, funções reutilizáveis, etc.).
- Se estiver criando um **back-end** ou **full-stack**, siga o padrão REST para a API.
- Não é necessário implementar autenticação de usuários, mas isso pode ser adicionado como bônus se desejar.

## 🛠️ Tecnologias Permitidas
- **Front-end**:
  - HTML, CSS, JavaScript puro.
  - Frameworks/libraries: React, Vue.js, Angular.
  
- **Back-end**:
  - **Node.js** (JavaScript ou TypeScript).
  - **Java** (Spring Boot).
  - **Python** (Flask).
  - **PHP** (Laravel).

## 📦 Como Entregar o Projeto
1. Crie um repositório no GitHub com o nome do seu projeto.
2. Coloque todo o código do projeto nesse repositório.
3. Faça um arquivo `README.md` explicando:
   - O que o projeto faz.
   - Como rodar o projeto localmente (instruções de instalação e execução).
   - As tecnologias utilizadas.
4. Inclua prints/screenshots do projeto rodando (se possível).

## 💡 Desafio Extra (Opcional)
Se você quiser se desafiar ainda mais, pode adicionar um **sistema de usuários**. Com isso, cada usuário teria suas próprias tarefas e seria necessário implementar:
- **Autenticação de usuários** (login e logout).
- **Cadastro de novos usuários**.
- **Teste**.
- Cada usuário só pode ver e gerenciar suas próprias tarefas.

Boa sorte! 🚀
