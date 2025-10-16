##Sistema de Gerenciamento de Produtos - Descrição

📋 Sobre o Projeto
Este é um sistema web completo desenvolvido em Spring Boot para gerenciamento de produtos, implementando um CRUD (Create, Read, Update, Delete) com arquitetura MVC (Model-View-Controller) e integração com banco de dados MySQL.

🎯 Funcionalidades Principais
✅ CRUD Completo
Cadastrar novos produtos no sistema

Listar todos os produtos cadastrados

Atualizar informações dos produtos existentes

Excluir produtos do sistema

🔍 Sistema de Pesquisa e Filtros
Pesquisa geral por qualquer termo (nome, descrição, categoria)

Filtro por categorias pré-definidas

Busca em tempo real com interface amigável

🗃️ Entidade Principal: Produto
A entidade Produto contém:

ID (auto-incremento)

Nome (obrigatório)

Descrição

Preço (obrigatório)

Quantidade em estoque (obrigatório)

Categoria

🏗️ Arquitetura MVC Implementada
Model (Produto.java)
Entidade JPA mapeada para tabela produtos

Anotações para persistência no banco

Validações e constraints

View (Templates Thymeleaf)
listar.html - Interface principal com lista e pesquisa

formulario.html - Formulário de cadastro/edição

Layout responsivo com Bootstrap 5

Controller (ProdutoController.java)
Gerencia rotas e requisições HTTP

Integração entre Model e View

Operações CRUD através de endpoints RESTful

Camadas Adicionais
Repository - Interface Spring Data JPA

Service - Camada de lógica de negócio

💾 Banco de Dados
MySQL com database databasepi

Configuração automática de tabelas via JPA/Hibernate

Script de dados iniciais opcional

🚀 Tecnologias Utilizadas
Backend: Spring Boot 3.2.0, Spring Data JPA, Spring MVC

Frontend: Thymeleaf, Bootstrap 5, HTML5

Banco de Dados: MySQL

Persistência: Hibernate/JPA

Build: Maven

📊 Endpoints da Aplicação
Método	URL	Descrição
GET	/produtos	Lista todos os produtos
GET	/produtos/novo	Formulário de cadastro
POST	/produtos/salvar	Salva/atualiza produto
GET	/produtos/editar/{id}	Formulário de edição
GET	/produtos/excluir/{id}	Exclui produto
GET	/produtos/pesquisar	Pesquisa produtos
GET	/produtos/categoria/{categoria}	Filtra por categoria
🎨 Interface do Usuário
Design responsivo e moderno com Bootstrap

Tabela dinâmica com lista de produtos

Formulários validados no frontend e backend

Sistema de alertas e confirmações

Navegação intuitiva entre funcionalidades

🔧 Configuração e Execução
Banco de dados MySQL com nome databasepi

Configuração de credenciais no application.properties

Execução via mvn spring-boot:run

Acesso em http://localhost:8080/produtos

📈 Próximas Evoluções
O projeto está preparado para expansão com:

Mais entidades (Clientes, Vendas, Fornecedores)

Sistema de autenticação e autorização

Relatórios e estatísticas

API REST para integração

Upload de imagens dos produtos
