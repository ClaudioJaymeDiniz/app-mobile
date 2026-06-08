# SmartForms

## Descrição

O **SmartForms** é um sistema completo para criação, gerenciamento e análise de formulários dinâmicos. A aplicação permite que usuários criem projetos, desenvolvam formulários personalizados e coletem respostas de forma estruturada, incluindo suporte a envio de imagens e visualização em dashboards.

O sistema foi projetado com foco em **usabilidade (no-code)**, **arquitetura limpa** e **suporte offline**, permitindo que dados sejam coletados mesmo sem conexão com a internet.

---

## Objetivo

Desenvolver uma aplicação mobile e backend capaz de:

* Criar formulários dinâmicos
* Gerenciar projetos e usuários
* Coletar respostas estruturadas
* Exibir dados analíticos em dashboards
* Funcionar em cenários offline

---

## Arquitetura do Sistema

O projeto segue os princípios de **Clean Architecture**, garantindo separação de responsabilidades:

```
📦 Projeto
├── core/           → Regras de negócio (Domain + Use Cases)
├── data/           → Implementações (Repositories, API, SQLite)
├── presentation/   → UI (React Native + Expo)
├── backend/        → API REST (FastAPI + PostgreSQL)
```

### 🔹 Backend

* API RESTful
* Autenticação com JWT
* Banco relacional (PostgreSQL / SUPABASE)
* ORM: Prisma
* Armazenamento de imagens em nuvem (planejado)

### 🔹 Mobile

* React Native + Expo
* TypeScript
* Expo Router
* Suporte offline com SQLite
* Sincronização de dados

---

## Planejamento por Sprints

---

## 🟢 Sprint 1 — MVP: Fundação do Sistema

🎯 Objetivo
Construir a base funcional do SmartPanel, permitindo que usuários criem projetos, montem formulários dinâmicos e coletem respostas pelo aplicativo mobile.

# ✅ Funcionalidades Entregues
Cadastro e autenticação de usuários

Login com e-mail e senha

Criação e organização de projetos

Criação de formulários dinâmicos

Campos configuráveis por tipo

Renderização dos formulários no mobile

Envio de respostas

Validação de campos obrigatórios

Armazenamento das respostas no backend

🛠️ Tecnologias Aplicadas

Autenticação com JWT

Estrutura de formulários baseada em JSON

API REST

React Native com Expo

Renderização dinâmica de campos

Banco de dados relacional no backend

## 🟡 Sprint 2 — Expansão: Controle e Gestão

 🎯 Objetivo

Evoluir o MVP para um sistema mais utilizável em cenários reais, adicionando controle de acesso, organização dos dados e recursos administrativos.

#✅ Funcionalidades Entregues

Formulários públicos e privados

Compartilhamento de formulários por link

Controle de acesso por usuário

Listagem de respostas recebidas

Visualização detalhada das respostas

Exportação de dados em CSV

Arquivamento de projetos e formulários

Lixeira com possibilidade de restauração

Separação entre dono do projeto e respondentes

Cache local de projetos e formulários

🛠️ Tecnologias Aplicadas

Controle de permissões no backend

Soft delete para arquivamento

Exportação de dados

Cache local no aplicativo

Integração entre frontend mobile e API


## 🔴 Sprint 3 — Final: Experiência Profissional e Uso Offline
 🎯 Objetivo
Finalizar o sistema com recursos avançados, melhor experiência para o usuário e preparação para uso real em campo, inclusive em cenários com internet instável.

# ✅ Funcionalidades Entregues
Dashboard analítico de respostas

Gráficos de barra, linha e pizza

Exportação de relatório em PDF

Upload de imagens nas respostas

Edição de formulários

Personalização visual dos projetos

Drag and drop para reorganização de campos

Sincronização offline com SQLite

Fila local de ações pendentes

Sincronização automática ao voltar a conexão

Cache local de projetos e formulários

Suporte a notificações push

Preparação para login social com Google

Preparação para build Android/APK

🛠️ Tecnologias Aplicadas

SQLite local com expo-sqlite

Fila de sincronização offline

SecureStore para sessão local

NetInfo para detecção de conexão

Geração de PDF no mobile

Gráficos com SVG

Upload de arquivos/imagens

Push notifications com Expo

Configuração Android com Expo

###  Tecnologias aplicadas

* Armazenamento em nuvem (Cloudinary/Firebase)
* Processamento assíncrono
* Geração de relatórios
* Integrações externas



---

## 📊 Funcionalidades Principais do SmartPanel
📁 Projetos organizados por usuário

🧩 Formulários dinâmicos

🔐 Autenticação com JWT

🧑‍🤝‍🧑 Controle de acesso público e privado

📱 Aplicativo mobile com Expo

📸 Upload de imagens nas respostas

📊 Dashboard analítico

📄 Relatórios em PDF

📤 Exportação em CSV

🗑️ Arquivamento e lixeira

🔄 Sincronização offline

💾 Cache local com SQLite

🔔 Suporte a notificações push

🎨 Personalização visual

🧱 Drag and drop de campos


---

## ⚙️ Requisitos Não Funcionais

* Arquitetura RESTful
* Banco de dados relacional (PostgreSQL)
* Armazenamento externo de mídia
* Autenticação segura com JWT
* Interface intuitiva (no-code)
* Performance em formulários longos
* Suporte offline
* Escalabilidade
* Conformidade com LGPD

---

## 🧪 Tecnologias Utilizadas

### 📱 Mobile

* React Native
* Expo
* TypeScript
* Expo Router

### 🌐 Backend

* Python (FastAPI)
* PostgreSQL
* Prisma ORM
* JWT Authentication

### 🛠️ Outros

* SQLite (offline-first)
* Axios
* Cloudinary / Firebase (planejado)

---

## ▶️ Como Executar o Projeto

### 🔹 Backend

```bash
# Instalar dependências
pip install -r requirements.txt

# Rodar servidor
uvicorn main:app --reload
```

---

### 🔹 Mobile

```bash
# Instalar dependências
npm install

# Rodar projeto
npx expo start
```

---

## 📌 Diferenciais do Projeto

* Arquitetura limpa e escalável
* Suporte offline-first
* Formulários dinâmicos (no-code)
* Sistema modular e extensível
* Preparado para crescimento (SaaS)

---

## 📈 Trabalhos Futuros

* Implementação completa de notificações
* Integração com serviços de e-mail
* Melhorias no dashboard (gráficos avançados)
* Sistema de colaboração em tempo real
* Deploy em ambiente cloud

---

## 👨‍💻 Autor

Claudio Jayme

---

## 📄 Licença

Este projeto é acadêmico e desenvolvido para fins educacionais.
