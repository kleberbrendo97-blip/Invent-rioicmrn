# PROJETO: Sistema de Inventário de Equipamentos de Som

## Objetivo

Desenvolver um sistema web profissional para gerenciamento completo do inventário de equipamentos de sonorização, permitindo controlar patrimônio, localização, empréstimos, manutenções, inventários e histórico de movimentações.

---

# Tecnologias

## Backend
- ASP.NET Core 9 (C#)
- Entity Framework Core
- SQL Server
- API REST
- JWT Authentication

## Frontend
- React + TypeScript
- Vite
- Bootstrap 5
- Axios
- React Router
- Chart.js

## Banco de Dados
SQL Server

---

# Arquitetura

Utilizar Clean Architecture contendo:

/Domain
/Application
/Infrastructure
/API
/Web
/Shared

Aplicar:

- Repository Pattern
- Unit of Work
- Dependency Injection
- DTOs
- AutoMapper
- FluentValidation
- Middleware de tratamento de erros
- Logging
- Versionamento da API

---

# Módulo de Login

Implementar autenticação utilizando JWT.

Perfis:

Administrador
Técnico
Operador
Consulta

Funcionalidades:

- Login
- Logout
- Recuperação de senha
- Alteração de senha
- Controle de permissões
- Bloqueio por tentativas

---

# Dashboard

Exibir:

Total de equipamentos

Disponíveis

Emprestados

Em manutenção

Baixados

Valor total do patrimônio

Gráfico por categoria

Gráfico por situação

Equipamentos com garantia vencendo

Últimas movimentações

---

# Cadastro de Equipamentos

Campos:

Id

Código Patrimonial

QR Code

Código de Barras

Categoria

Marca

Modelo

Número de Série

Descrição

Patrimônio

Localização

Setor

Responsável

Fornecedor

Data da Compra

Valor

Garantia

Situação

Estado de Conservação

Observações

Foto Principal

Fotos Adicionais

Documentos

Manual

Nota Fiscal

---

# Categorias

Mesa Digital

Mesa Analógica

Caixa Ativa

Caixa Passiva

Subwoofer

Monitor

Microfone com fio

Microfone sem fio

Headset

Retorno

Direct Box

Amplificador

Processador Digital

Equalizador

Compressor

Notebook

Projetor

Câmera

Pedestal

Rack

Cabos XLR

Cabos P10

Cabos HDMI

Cabos Speakon

Extensões

Instrumentos

Iluminação

Acessórios

Outros

---

# Localização

Cadastrar:

Igreja

Auditório

Palco

Sala Técnica

Depósito

Veículo

Eventos

Outros

---

# Movimentações

Registrar:

Entrada

Saída

Transferência

Empréstimo

Devolução

Manutenção

Baixa

Cada movimentação deve registrar:

Data

Usuário

Destino

Responsável

Evento

Motivo

Observações

Assinatura Digital

---

# Empréstimos

Registrar:

Solicitante

Telefone

Documento

Destino

Evento

Data de retirada

Data prevista

Data devolução

Status

Checklist

Fotos

Termo de responsabilidade em PDF

---

# Manutenção

Registrar:

Equipamento

Problema

Diagnóstico

Tipo

Preventiva

Corretiva

Fornecedor

Técnico

Valor

Peças utilizadas

Data Entrada

Data Saída

Garantia do serviço

Status

Anexos

---

# Inventário

Criar inventários periódicos.

Registrar:

Responsável

Data

Local

Equipamentos encontrados

Equipamentos não encontrados

Divergências

Observações

Gerar relatório final.

---

# Pesquisa

Pesquisar por qualquer campo.

Filtros:

Categoria

Marca

Modelo

Situação

Local

Responsável

Fornecedor

Garantia

Código

QR Code

Código de Barras

---

# Relatórios

Gerar em:

PDF

Excel

CSV

Relatórios:

Patrimônio Geral

Inventário

Movimentações

Empréstimos

Equipamentos por Categoria

Equipamentos por Local

Equipamentos em Manutenção

Garantias

Equipamentos Baixados

Valor do Patrimônio

---

# QR Code

Gerar automaticamente.

Leitura utilizando câmera.

Consultar equipamento pelo QR Code.

---

# Etiquetas

Gerar etiquetas contendo:

Logo

Nome

Código

QR Code

Patrimônio

Modelo

---

# Uploads

Permitir:

Fotos

PDF

Vídeos

Manuais

Notas Fiscais

Garantias

---

# Auditoria

Registrar:

Usuário

Data

IP

Ação

Tabela

Valor Antigo

Valor Novo

---

# API REST

Criar endpoints completos:

GET

POST

PUT

DELETE

PATCH

Documentar utilizando Swagger.

---

# Segurança

JWT

Refresh Token

Criptografia de senha

HTTPS

CORS

CSRF

Proteção contra SQL Injection

Proteção contra XSS

Validação de dados

Logs

---

# Interface

Tema moderno

Modo Claro

Modo Escuro

Menu lateral

Dashboard

Cards

Gráficos

Tabela com paginação

Pesquisa instantânea

Filtros avançados

Upload por arrastar arquivos

Totalmente responsivo

---

# Banco de Dados

Criar automaticamente todas as tabelas.

Criar:

Migrations

Seeds

Relacionamentos

Índices

Procedures quando necessário.

---

# Extras

Backup automático

Importação via Excel

Exportação para Excel

Importação CSV

Notificações

E-mail

WhatsApp

Garantia vencendo

Equipamento parado há muito tempo

---

# Qualidade

Utilizar SOLID.

Utilizar Clean Code.

Utilizar Design Patterns.

Código comentado.

Separação por camadas.

Testes unitários.

Testes de integração.

README completo.

Docker Compose.

Arquivo .env.

Scripts de instalação.

Projeto pronto para produção.

Todo o código deve ser organizado, escalável, seguro, documentado e seguir as melhores práticas de desenvolvimento profissional.
