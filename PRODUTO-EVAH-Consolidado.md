# 📦 PRODUTO EVAH/AIVAH - Informações Consolidadas

> **Objetivo:** Este documento consolida todas as informações sobre o produto EVAH/AIVAH (assistente virtual) extraídas dos arquivos do projeto.

---

## 🎯 1. DEFINIÇÃO E CONCEITO DO PRODUTO

### 1.1 Nome e Identidade
- **Nome Técnico:** AIVAH (Assistente Inteligente de Vendas Automatizado para Humanos)
- **Nome Comercial:** EVAH (Ecossistema de Valor Automatizado para Humanos)
- **Apresentação ao Cliente:** Pode variar (ex: BiraBot para Bira Veículos)
- **Framework Base:** VIAH (Vendas Inteligentes Automatizadas para Humanos)

### 1.2 Visão Geral
O **EVAH/AIVAH** é a camada central de inteligência da plataforma **VIAH**. Vai além de uma assistente conversacional: integra módulos, conecta sistemas, automatiza fluxos e coordena operações em um ponto único entre **VIAH ERP**, automações e serviços externos.

**Principais Características:**
- Consolida informações
- Organiza processos
- Antecipa necessidades
- Atua como suporte inteligente (não substitui o operador humano)
- Acelera rotinas
- Mantém tudo alinhado para que o time foque no que realmente exige análise, decisão e relacionamento

### 1.3 Posicionamento no Ecossistema VIAH
- **VIAH** = Framework modular completo
- **EVAH/AIVAH** = Assistente conversacional inteligente (produto principal)
- Pode ser usado como módulo do VIAH ou como solução independente

---

## 🔧 2. FUNCIONALIDADES E CAPACIDADES

### 2.1 Integração Multicanal
**Canais Suportados:**
- WhatsApp
- Instagram
- Facebook Messenger
- Telegram
- WebChat do site
- Qualquer canal que o cliente queira integrar

**Capacidades:**
- Centralização de mensagens de todos os canais
- Execução de fluxos automatizados consistentes
- Encaminhamento para atendentes humanos quando necessário
- Integração com processos internos e automações do negócio
- Atendimento integrado e consistente em todos os canais

### 2.2 Atendimento com Inteligência Artificial
**Provedores de IA Suportados:**
- OpenAI (ChatGPT)
- Google Gemini
- IBM Watson

**Capacidades:**
- Geração de respostas contextualizadas e naturais
- Análise de sentimentos em tempo real
- Interpretação de diferentes tipos de dados (estruturados e não estruturados)
- Automação dinâmica de processos dentro da conversa
- Entender e interpretar consultas abertas e variadas
- Gerar respostas contextuais e personalizadas
- Executar decisões e acionar automações conforme regras de negócio
- Encaminhar para atendimento humano quando necessário
- Redirecionar para atendimento guiado quando apropriado

### 2.3 Atendimento Guiado
**Funcionalidades:**
- Conduz o cliente por fluxos personalizados
- Coleta informações de forma organizada
- Realiza validações durante a interação
- Preenche agendas automaticamente
- Executa automações essenciais ao atendimento
- Ideal para formulários, fichas e coletas de informações
- Adapta fluxos conversacionais conforme necessidade da empresa
- Coleta inteligente de dados em tempo real
- Integração com agendas e processos internos

**Casos de Uso:**
- Triagem automatizada
- Coleta de cadastros e preferências
- Consultas de estoque, status de pedidos, agendamentos
- Agendamentos automatizados com controle de horários

### 2.4 Consultas via Web Scraping
**Capacidades:**
- Acessa páginas externas e extrai dados em tempo real
- Coleta preços, prazos, status ou disponibilidade de serviços
- Extração de informações de sites e portais
- Integração direta às automações do atendimento
- Dados externos transformados em respostas imediatas
- Enriquecimento do atendimento com dados externos confiáveis

**Exemplos:**
- Consulta de anúncios (OLX, Webmotors, etc.)
- Extração de dados de links enviados pelo cliente

### 2.5 Transcrições de Áudio para Texto
**Funcionalidades:**
- Recebe mensagens de voz em canais compatíveis
- Transforma áudio em texto automaticamente
- Permite interpretação e processamento do conteúdo
- Suporte a múltiplos canais de comunicação
- Armazenamento seguro das mensagens para consultas futuras
- Facilita interação sem depender de digitação manual

**Tecnologias:**
- Whisper API ou OpenAI para transcrição

### 2.6 Consultas na Tabela FIPE
**Funcionalidades:**
- Busca informações atualizadas diretamente da Tabela FIPE
- Oferece dados precisos para negociações automotivas
- Suporte a consultas rápidas durante o atendimento
- Integração com fluxos de vendas e negociações
- Informação confiável para decisões comerciais

### 2.7 Agendamentos via Google Calendar
**Funcionalidades:**
- Sincroniza e gerencia eventos diretamente no Google Calendar
- Criação automática de eventos
- Consulta rápida de horários disponíveis
- Notificações integradas para clientes e equipe
- Integração direta com fluxos de atendimento e processos internos
- Evita conflitos de horários
- Garante registro e acompanhamento de compromissos

---

## 🤖 3. AGENTES E MÓDULOS ESPECIALIZADOS

### 3.1 Agente CRM
**Funcionalidades Principais:**
- Captura automática de leads no primeiro contato
- Verificação de duplicidade por e-mail ou telefone
- Identificação automática e enriquecimento de dados do lead
- Criação, atualização e gestão automática de leads no CRM (Odoo)
- Classificação automática por prioridade e intenção de compra
- Status: Quente, Morno, Frio, Em Atendimento
- Execução de campanhas segmentadas (follow-ups, mensagens automáticas)
- Roteamento inteligente de leads qualificados para atendimento humano
- Geração de relatórios e dashboards
- Atualização instantânea da interface do Odoo

**Funcionalidades Opcionais:**
- Agendamento automático de compromissos
- Pontuação automática de leads (lead scoring)
- Integração com qualquer CRM via API

### 3.2 Agente Calendar
**Funcionalidades:**
- Agendar eventos no Google Calendar
- Atualizar compromissos
- Remarcar eventos
- Cancelar eventos
- Consultar agenda e verificar disponibilidade
- Enviar lembretes e solicitações de confirmação
- Validação de horários (evitar conflitos)

### 3.3 Agente de Transcrição (Texto ↔ Áudio)
**Funcionalidades:**
- Converter texto em áudio (para envio de áudios pelo WhatsApp)
- Converter áudio em texto (para processamento)
- Suporte a múltiplos canais

### 3.4 Agente de Consulta SQL Odoo
**Funcionalidades:**
- Consultar produtos na base de dados do Odoo
- Consultar informações de clientes
- Consultar pedidos e status
- Integração direta com ERP

### 3.5 Agente de Detalhes do Produto
**Funcionalidades:**
- Mostrar detalhes completos de produtos/serviços
- Consultar mídias dos produtos do Odoo
- Apresentar informações enriquecidas (veículos, serviços, etc.)

### 3.6 Agente Gateway de Pagamento
**Funcionalidades:**
- Permitir pagamentos via API Gateway
- Integração com gateways de pagamento
- Processamento de transações

### 3.7 Agente Mídias pelo WhatsApp
**Funcionalidades:**
- Enviar mídias (áudio, imagem e vídeo) pelo WhatsApp
- Receber e processar mídias enviadas pelo cliente

### 3.8 Agente Obter Localização pelo CEP
**Funcionalidades:**
- Solicitar CEP ao cliente
- Detectar localização pelo Google Maps
- Usar localização para personalização de atendimento

### 3.9 Agente Qualificar Lead
**Funcionalidades:**
- Criar lead automaticamente
- Qualificar lead com base em interações
- Classificar por interesse e potencial

### 3.10 Agente Adaptar ao Negócio do Cliente
**Funcionalidades:**
- Adaptar-se à realidade do negócio do cliente
- Personalizar fluxos conforme segmento
- Ajustar linguagem e abordagem

---

## 🏗️ 4. ARQUITETURA E TECNOLOGIAS

### 4.1 Stack Tecnológico
**Orquestração:**
- **n8n** - Automação e orquestração de fluxos

**Memória e Contexto:**
- **Zep** - Memória conversacional e histórico

**IA e Processamento:**
- **OpenAI (ChatGPT)** - Processamento de linguagem natural
- **Google Gemini** - IA alternativa
- **IBM Watson** - IA alternativa
- **Whisper API** - Transcrição de voz

**Integrações:**
- **Evolution API** - Integração WhatsApp
- **Meta API** - WhatsApp, Messenger, Instagram
- **Telegram API**
- **Google Calendar API**
- **Odoo ERP** - CRM e gestão

**Infraestrutura:**
- **Docker Swarm ou Kubernetes** - Orquestração
- **PostgreSQL** - Banco de dados
- **MinIO ou S3** - Armazenamento de arquivos
- **Node.js ou Python** - Backend

### 4.2 Arquitetura Modular no N8N
**Fluxo Geral:**
1. **1_Main_EntradaMensagem** - Entrada de texto, áudio ou imagem
2. **2_TratamentoMensagem** - Converte áudio, texto, imagem em texto limpo
3. **3_Orquestrador** - Detecta a intenção do cliente
4. **4_RoteadorDeAgentes** - Direciona para o agente correto
5. **Agentes Específicos:**
   - 5_AgenteBoasVindas
   - 6_AgenteConsultaVeiculos
   - 7_AgenteWebScraping
   - 8_AgenteAgendamento
   - 9_AgenteCRM
   - 10_AgenteDesconhecido (Fallback)

### 4.3 Camadas da Arquitetura
1. **Camada de Entrada (Front-End de Comunicação)**
   - WhatsApp, Webchat (VIAH Chat)
   
2. **Camada de Inteligência**
   - VIAH Chat (Typebot) - Interface guiada
   - VIAH AIVAH - Assistente de IA
   
3. **Camada de Automações**
   - VIAH Conductor (n8n) - Executa lógicas de negócio
   - VIAH Connect - Ponte entre canais externos e módulos internos
   
4. **Camada de Backend e Gestão**
   - VIAH Omni (Chatwoot) - Atendentes humanos
   - VIAH ERP (Odoo) - Registro e gestão

---

## 🎯 5. CASOS DE USO E OBJETIVOS

### 5.1 Objetivos do Assistente
**Comunicação Inicial:**
- Detectar e responder saudações
- Apresentar-se e explicar função

**Coleta de Interesse:**
- Identificar tipo de produto/serviço desejado
- Extrair informações específicas (marca, modelo, tipo, ano, preço, etc.)

**Consulta de Produtos:**
- Integrar com banco de dados
- Apresentar resultados baseados em filtros

**Registro e Qualificação de Lead:**
- Criar lead no início do atendimento
- Atualizar lead conforme mais dados são fornecidos
- Integrar com CRM Odoo

**Agendamento:**
- Perguntar disponibilidade do cliente
- Registrar data e hora sugerida
- (Futuramente) integrar com agenda de vendedores

**Interpretação Multimídia:**
- **Áudio:** Transcrever voz em texto
- **Imagem:** Extrair dados visuais, consultar produtos semelhantes
- **Link:** Extrair dados de anúncios, realizar consulta no banco

**Memória e Contexto:**
- Usar memória (Zep) para manter histórico
- Entender contexto conversacional
- Exemplo: "Quero um carro de 2022" + "quero que seja SUV" → entender busca completa

### 5.2 Dores que o EVAH Resolve

**Problemas Operacionais:**
- Tempo de resposta lento
- Sobrecarga da equipe de atendimento
- Dificuldade em atender fora do horário comercial
- Alto custo com equipe de suporte
- Baixa escalabilidade

**Problemas de Experiência do Cliente:**
- Frustração do cliente (demora, falta de agilidade)
- Perda de oportunidades de venda
- Atendimento inconsistente
- Falta de personalização
- Menor conveniência

**Problemas Estratégicos:**
- Menor competitividade
- Falta de dados sobre clientes
- Dificuldade em nutrir leads
- Imagem antiquada da empresa
- Menor fidelização

---

## 📋 6. REQUISITOS E PRÉ-REQUISITOS

### 6.1 Infraestrutura
- Servidor Linux (Docker Swarm ou Kubernetes)
- Banco de dados PostgreSQL
- Armazenamento de arquivos (MinIO ou S3)

### 6.2 Ferramentas Principais
- n8n instalado e configurado
- IA (LLM): GPT-5 API ou modelo local (Llama 3, Mistral)
- Node.js ou Python para backend

### 6.3 Integrações Obrigatórias
- APIs de comunicação (Meta API, Evolution API, Telegram)
- CRM (Odoo, HubSpot, Pipedrive)
- Provedores de envio de mensagens (SMTP, Twilio, Z-API)

### 6.4 Credenciais Necessárias
- Google Cloud (para Google Calendar API)
- OpenAI (API Key)
- OAuth 2.0 Client ID (Google Calendar)
- Credenciais de APIs de comunicação

---

## 🚀 7. MVP E DESENVOLVIMENTO

### 7.1 Funcionalidades MVP
**Prioritárias:**
- Gestão mínima de leads
- Fluxo completo de atendimento
- Notificações básicas (som, push, e-mail)
- Integração com WhatsApp
- Atendimento guiado básico
- Integração com Odoo CRM

**Agentes Essenciais para MVP:**
- Agente Transcrição de mensagens (texto ↔ áudio)
- Agente CRM
- Agente Calendar
- Fluxo de atendimento guiado para coleta de dados

### 7.2 Melhorias e Correções Necessárias
- Quando é mandado um texto em duas linhas, dá falha (interpreta errado)
- Quando o cliente manda texto com "aspas" dá erro no agente de transcrição
- Precisa ter ferramenta que faça tratamento da mensagem antes de passar para os agentes
- Reorganizar os sub-agentes para atendimento
- Configurar memória RAG na EVAH

### 7.3 Funcionalidades Futuras
- Assistente específico para o logista (empresa) para gerenciar áreas da empresa via agente
- Integração com agenda de vendedores
- Melhorias em interpretação de imagens
- Expansão de integrações

---

## 📊 8. MÉTRICAS E MONITORAMENTO

### 8.1 Métricas de Desempenho
- Número de leads por canal
- Taxa de conversão
- Leads quentes vs frios
- Performance de campanhas
- Tempo de resposta
- Taxa de resolução automática

### 8.2 Dashboards e Relatórios
- Relatórios de performance
- Acompanhamento de conversão
- Status dos leads
- Métricas de atendimento
- Alertas para leads de alta prioridade

---

## 🔄 9. INTEGRAÇÕES COM OUTROS MÓDULOS VIAH

### 9.1 VIAH ERP (Odoo)
- Integração nativa para consulta de produtos
- Registro de leads e oportunidades
- Consulta de estoque e pedidos
- Sincronização de dados

### 9.2 VIAH Omni (Chatwoot)
- Encaminhamento para atendimento humano
- Histórico centralizado
- Gestão de conversas

### 9.3 VIAH Conductor (n8n)
- Execução de automações
- Orquestração de fluxos
- Integração com sistemas externos

### 9.4 VIAH Connect
- Conexão com canais externos
- Integração com APIs de mercado

---

## 📝 10. NOTAS E OBSERVAÇÕES

### 10.1 Nomenclatura
- Há variação entre "AIVAH" e "EVAH" nos documentos
- "AIVAH" parece ser o nome técnico
- "EVAH" parece ser o nome comercial/apresentação
- Pode ter nomes customizados por cliente (ex: BiraBot)

### 10.2 Adaptabilidade
- O EVAH deve ser capaz de se adaptar à realidade do negócio do cliente
- Personalização por segmento e contexto
- Flexibilidade para diferentes casos de uso

### 10.3 Foco no MVP
- Priorizar funcionalidades essenciais
- Garantir estabilidade e confiabilidade
- Focar em casos de uso principais
- Demonstrar valor imediato

---

**Última atualização:** 2025  
**Fonte:** Consolidação de múltiplos arquivos do projeto

