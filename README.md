# 🧪 Laboratório: Criação de Instância Gerenciada de SQL no Microsoft Azure

Este repositório documenta o processo de criação e configuração de uma Instância Gerenciada de SQL no Microsoft Azure, com o objetivo de praticar e consolidar conhecimentos sobre a plataforma.

## 📋 Sumário

- [🎯 Objetivo](#-objetivo)
- [🛠️ Pré-requisitos](#-pré-requisitos)
- [🚀 Passo a Passo](#-passo-a-passo)
  - [1. Acessar o Portal do Azure](#1-acessar-o-portal-do-azure)
  - [2. Criar uma Nova Instância Gerenciada de SQL](#2-criar-uma-nova-instância-gerenciada-de-sql)
  - [3. Configurar os Detalhes da Instância](#3-configurar-os-detalhes-da-instância)
  - [4. Configurar a Rede Virtual e Sub-rede](#4-configurar-a-rede-virtual-e-sub-rede)
  - [5. Revisar e Criar](#5-revisar-e-criar)
  - [6. Monitorar o Progresso da Implantação](#6-monitorar-o-progresso-da-implantação)
  - [7. Conectar-se à Instância](#7-conectar-se-à-instância)
- [💡 Dicas e Observações](#-dicas-e-observações)
- [📚 Referências](#-referências)

## 🎯 Objetivo

Praticar o processo de criação e configuração de uma Instância Gerenciada de SQL na plataforma Microsoft Azure, documentando cada etapa para facilitar revisões futuras e auxiliar outros estudantes ou profissionais interessados no tema.

## 🛠️ Pré-requisitos

- Conta ativa no [Microsoft Azure](https://azure.microsoft.com/pt-br/free/)
- Acesso ao [Portal do Azure](https://portal.azure.com/)
- Permissões adequadas para criar recursos no Azure

## 🚀 Passo a Passo

### 1. Acessar o Portal do Azure

- Navegue até [https://portal.azure.com](https://portal.azure.com) e faça login com sua conta Microsoft.

### 2. Criar uma Nova Instância Gerenciada de SQL

- No menu lateral, clique em **"SQL do Azure"**.
- Clique em **"+ Criar"** para iniciar o processo de criação.

### 3. Configurar os Detalhes da Instância

- **Assinatura**: Selecione sua assinatura do Azure.
- **Grupo de Recursos**: Crie um novo ou selecione um existente.
- **Nome da Instância Gerenciada**: Escolha um nome único.
- **Região**: Selecione a região mais próxima de você.
- **Método de Autenticação**: Escolha entre Autenticação do SQL ou Microsoft Entra.
- **Login de Administrador**: Defina um nome de usuário e senha seguros.

### 4. Configurar a Rede Virtual e Sub-rede

- **Rede Virtual (VNet)**: Crie uma nova ou selecione uma existente.
- **Sub-rede**: Crie uma nova sub-rede dedicada para a instância gerenciada.

> **Nota**: A sub-rede deve ser delegada à Instância Gerenciada de SQL do Azure.

### 5. Revisar e Criar

- Clique em **"Revisar + criar"**.
- Após a validação, clique em **"Criar"** para iniciar a implantação da instância.

### 6. Monitorar o Progresso da Implantação

- Acompanhe o progresso da implantação através do ícone de **Notificações** no portal do Azure.
- Após a conclusão, acesse o grupo de recursos para visualizar a instância criada.

### 7. Conectar-se à Instância

- Para se conectar à instância, utilize ferramentas como o **SQL Server Management Studio (SSMS)** ou **Azure Data Studio**.
- Certifique-se de que a máquina cliente esteja na mesma VNet ou configure uma conexão VPN ponto a site.

## 💡 Dicas e Observações

- **Segurança**: Configure regras de firewall e grupos de segurança de rede (NSG) adequados para proteger sua instância.
- **Custos**: Monitore o uso da instância para evitar cobranças inesperadas. Considere parar a instância quando não estiver em uso.
- **Automatização**: Explore o uso de [Azure CLI](https://learn.microsoft.com/pt-br/cli/azure/install-azure-cli) ou [PowerShell](https://learn.microsoft.com/pt-br/powershell/azure/new-azureps-module-az?view=azps-10.0.0) para automatizar a criação e gerenciamento de recursos.


## 📚 Referências

- [Início Rápido – Criar uma Instância Gerenciada de SQL do Azure](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/instance-create-quickstart)
- [Documentação da Instância Gerenciada de SQL do Azure](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/)
- [Visão Geral da Instância Gerenciada de SQL do Azure](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/sql-managed-instance-paas-overview)

---

*Este projeto foi desenvolvido como parte do aprendizado em ciência de dados e infraestrutura na nuvem, visando a aplicação prática dos conhecimentos adquiridos.*
