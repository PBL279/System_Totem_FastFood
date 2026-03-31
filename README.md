# 🍔 **Totem Fast Food JK Burguer**

Sistema de autoatendimento para fast food desenvolvido como projeto acadêmico, com backend em **Spring Boot** e frontend em **React**. O sistema oferece uma experiência interativa e ágil, permitindo que os clientes façam pedidos diretamente em um totem, com opções de combos e um sistema de fidelização via CPF.

## 📌 **Objetivo do Projeto**

O objetivo deste projeto é desenvolver um sistema de **autoatendimento** em um **totem** para fast food. O sistema tem como diferencial um sistema de **fidelização** baseado em CPF, permitindo que os clientes acumulem pontos e ganhem benefícios como descontos e brindes.

Além disso, o sistema visa:

* **Reduzir filas e melhorar a experiência do cliente**
* **Automatizar o processo de pedido**
* **Oferecer um sistema intuitivo e ágil para os clientes**

---

## 🛠️ **Tecnologias Utilizadas**

### **Backend**:

* **Java 21**
* **Spring Boot 4.0.3**
* **Spring Data JPA** (para integração com o banco de dados MySQL)

### **Frontend**:

* **React 19.2**
* **React Router** (para navegação entre páginas)

### **Banco de Dados**:

* **Comand Line MySQL 8.3**

### **Ferramentas de Versionamento**:

* **Git** e **GitHub** (para controle de versão e colaboração)
* **Jira** (para gerenciamento de tarefas e sprints)

---

## 📋 **Funcionalidades**

* **Visualizar Cardápio**: O cliente pode visualizar as opções de produtos (lanches, bebidas, acompanhamentos, sobremesas) disponíveis no sistema.
* **Escolher Produtos**: Seleção de produtos, com opções de combos e componentes adicionais.
* **Fidelização via CPF**: O cliente pode inserir seu CPF para acumular pontos, obter descontos e participar de sorteios.
* **Pagamento**: O sistema oferece múltiplas formas de pagamento, incluindo **Pix**, **Cartão de Débito** e **Cartão de Crédito**.
* **Resumo do Pedido**: Exibe todos os itens do pedido, totalizando o valor para que o cliente finalize a compra.
* **Nota Fiscal**: Após o pagamento, o cliente recebe a nota fiscal e tem a opção de imprimir.

---

## 🚀 **Como Rodar o Projeto**

### **Pré-requisitos**:

Certifique-se de ter as seguintes ferramentas instaladas:

* **Java 17** ou superior
* **Node.js** (para o frontend)
* **MySQL 8**
* **Maven** ou **Gradle** (para o backend)

### **Rodando o Backend**:

1. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/totem-fast-food.git
   cd totem-fast-food/backend
   ```

2. Crie um banco de dados no MySQL:

   ```sql
   CREATE DATABASE totem_db CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
   ```

3. Execute o Spring Boot:

   ```bash
   ./mvnw spring-boot:run
   ```

4. O backend estará rodando na porta `8080` por padrão.

### **Rodando o Frontend**:

1. Navegue até o diretório do frontend:

   ```bash
   cd totem-fast-food/frontend
   ```

2. Instale as dependências:

   ```bash
   npm install
   ```

3. Inicie o servidor de desenvolvimento:

   ```bash
   npm start
   ```

4. O frontend estará acessível em `http://localhost:3000`.

---

## 🔑 **Estrutura do Projeto**

```plaintext
totem-fast-food/
├── backend/               # Backend em Spring Boot
│   ├── src/               # Código fonte do backend
│   ├── application.properties  # Configurações do Spring Boot
│   └── pom.xml            # Dependências do Maven
├── frontend/              # Frontend em React
│   ├── public/            # Arquivos públicos (index.html)
│   ├── src/               # Código fonte do React
│   ├── package.json       # Dependências do Node.js
└── README.md              # Este arquivo
```

---

## 📝 **Requisitos**

### **Requisitos Funcionais**:

* **RF1**: Permitir visualizar o cardápio.
* **RF2**: Selecionar produtos e montar o pedido.
* **RF3**: Inserir CPF para fidelização.
* **RF4**: Aplicar descontos e acumular pontos.
* **RF5**: Registrar o pedido e finalizar a compra.

### **Requisitos Não Funcionais**:

* **RNF1**: O sistema deve ser intuitivo e fácil de usar.
* **RNF2**: O sistema deve carregar as informações do cardápio em até 3 segundos.
* **RNF3**: O sistema deve ser seguro para o armazenamento de dados do cliente.
* **RNF4**: O sistema deve estar disponível 24/7, com 99% de uptime.

---

## 📄 **Diagrama de Banco de Dados**

O banco de dados do sistema foi estruturado em diversas tabelas que se relacionam entre si. As principais tabelas incluem:

* **Cliente**: Armazena informações do usuário, como CPF e pontos acumulados.
* **Produto**: Representa os itens disponíveis no cardápio.
* **Pedido**: Registra os pedidos feitos pelos clientes.
* **ItemPedido**: Relaciona os produtos com os pedidos.
* **Categoria**: Organiza os produtos por tipo (lanches, bebidas, etc.).

## 🔒 **Licença**

Este projeto está licenciado sob a **MIT License**.