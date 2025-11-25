Funcionalidades

O Agente Calendar será sistema objetivo e funcional que permite ao usuário gerenciar compromissos de forma simples e eficiente. Ele deve ser capaz de:

Agendar, atualizar, remarcar e cancelar eventos no Google Calendar.

Consultar a agenda e verificar disponibilidade de horários.

Enviar lembretes e solicitações de confirmação para o usuário e participantes, garantindo que todos os compromissos sejam acompanhados de forma prática e confiável.

Pré-requisitos

1. Infraestrutura / Ferramentas

Conta no Google Cloud (para criar projetos e usar Google Calendar API)

Conta na OpenAI (para usar GPT ou modelos de interpretação de linguagem natural)

n8n instalado e configurado (local ou servidor) para orquestração do fluxo

Navegador ou terminal para testes (localhost ou ambiente de produção)

Sistema de armazenamento seguro para credenciais (Google OAuth JSON e API Key da OpenAI)

2. APIs e Credenciais

Google Calendar

Criar projeto no Google Cloud

Ativar Google Calendar API

Criar OAuth 2.0 Client ID (Web ou Desktop)

Adicionar URIs de redirecionamento (teste local e produção)

Baixar JSON com Client ID e Client Secret

OpenAI

Criar conta na OpenAI

Gerar API Key secreta

Configurar sistema para usar a chave de forma segura

3. Lógica e Fluxo do Agente

Definir ações principais: agendar, atualizar, cancelar, consultar compromissos

Criar prompt base para interpretar comandos do usuário em linguagem natural

Implementar validação de horários: evitar conflitos e



Configuração do Google Calendar – Criação da API

1. Criar projeto no Google Cloud

Acesse o Google Cloud Console.

Clique em Criar Projeto.

Dê um nome relevante ao projeto (ex: AgenteCalendar).

Clique em Criar.

2. Ativar API do Google Calendar

No menu lateral, vá em APIs & Serviços → Biblioteca.

Pesquise por Google Calendar API.

Clique em Ativar.

3. Criar credenciais OAuth 2.0

Vá em APIs & Serviços → Credenciais → Criar Credenciais → OAuth 2.0 Client ID.

Tipo de aplicativo: Web Application (ou Desktop, dependendo do uso).

Adicione URIs de redirecionamento:

Para teste local: <http://localhost:5678/oauth2callback> (ou porta usada pelo seu app).

Para produção: URL do servidor que vai usar a API.

Clique em Criar.

Baixe o arquivo JSON com Client ID e Client Secret.

Guarde o arquivo com segurança; será usado para autenticação na API.

Configuração da OpenAI – API Key

1. Criar conta na OpenAI

Acesse OpenAI.

Crie uma conta ou faça login.

2. Gerar API Key

No menu, vá em View API Keys.

Clique em Create new secret key.

Copie a chave gerada e guarde em local seguro.

Esta chave será usada para autenticação em chamadas à API.

3. Uso da API

A API será utilizada para interpretar comandos em linguagem natural do usuário.

Ela deve receber texto do usuário e retornar intenção e parâmetros estruturados, como:

{
  "acao": "agendar",
  "titulo": "Reunião com João",
  "data": "2025-09-19",
  "hora": "10:00",
  "participantes": []
}