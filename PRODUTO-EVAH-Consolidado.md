# 📦 PLATAFORMA EVAH E EVAH ASSISTANT - Informações Consolidadas

> **Objetivo:** Este documento consolida todas as informações sobre a plataforma EVAH e o Evah Assistant (assistente virtual padrão) extraídas dos arquivos do projeto.

---

## 🎯 1. DEFINIÇÃO E CONCEITO DO PRODUTO

### 1.1 Nome e Identidade
- **EVAH** = Plataforma completa de IA (sistema completo que integra módulos, agentes, fluxos, orquestração, integrações e recursos avançados de atendimento)
- **Evah Assistant** = Assistente inteligente padrão da plataforma EVAH
- **Apresentação ao Cliente:** Cada cliente pode personalizar sua própria assistente (ex: BiraBot para Bira Veículos) sem impactar a identidade principal da plataforma EVAH

### 1.2 Visão Geral
**EVAH** é a plataforma completa de IA que integra módulos, agentes, fluxos, orquestração, integrações e recursos avançados de atendimento.

**Evah Assistant** é a assistente inteligente padrão da plataforma EVAH. Vai além de uma assistente conversacional: integra módulos, conecta sistemas, automatiza fluxos e coordena operações em um ponto único entre **EVAH ERP**, automações e serviços externos.

**Principais Características:**
- Consolida informações
- Organiza processos
- Antecipa necessidades
- Atua como suporte inteligente (não substitui o operador humano)
- Acelera rotinas
- Mantém tudo alinhado para que o time foque no que realmente exige análise, decisão e relacionamento

### 1.3 Posicionamento Estratégico
- **EVAH** = Plataforma completa de IA (sistema completo)
- **Evah Assistant** = Assistente inteligente padrão da plataforma (produto principal)
- Cada cliente pode personalizar sua própria assistente sem impactar a identidade principal da plataforma EVAH

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
- OpenAI Vision ou modelo customizado para leitura de imagens
- Playwright / Puppeteer / Cheerio para web scraping

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
- Atualizar compromissos
- Remarcar eventos
- Cancelar eventos
- Enviar lembretes e solicitações de confirmação

### 2.8 Gestão de Arquivos via Google Drive
**Funcionalidades:**
- Permite que o Evah Assistant gerencie arquivos no Google Drive do cliente
- Upload, download e organização de arquivos
- Controle de permissões via API oficial Google Drive
- Integração direta com fluxos de atendimento

### 2.9 Identificação de Conteúdo de Imagens
**Funcionalidades:**
- Permite que o Evah Assistant analise imagens enviadas por usuários
- Reconhecimento de elementos visuais, textos ou padrões relevantes
- Uso de OCR (reconhecimento óptico de caracteres) para extrair texto de imagens
- Consulta de produtos semelhantes com base em imagens
- Extração de dados visuais (modelo, tipo, cor) de veículos ou produtos

### 2.10 Consulta de Produtos no Estoque do ERP
**Funcionalidades:**
- Permite que o Evah Assistant consulte em tempo real a disponibilidade de produtos no ERP
- Exibe quantidade, localização e status do estoque
- Integração direta com EVAH ERP (Odoo) ou ERP do cliente
- Consultas via API com segurança e controle de acesso

### 2.11 Consulta de Detalhes de Produto
**Funcionalidades:**
- Habilita o Evah Assistant a retornar informações específicas de um produto com base na seleção do usuário
- Descrição, especificações técnicas, preços e variantes
- Consulta de mídias dos produtos do Odoo
- Apresentação de informações enriquecidas (veículos, serviços, etc.)

### 2.12 Exibição de Fotos de Produtos
**Funcionalidades:**
- Capacita o Evah Assistant a apresentar imagens associadas ao produto consultado
- Melhora a experiência visual do atendimento
- Consulta de mídias dos produtos do ERP

### 2.13 Wiki de Empresa
**Funcionalidades:**
- Determina todas as informações da empresa
- Base de conhecimento integrada ao assistente
- Permite respostas baseadas em informações institucionais

### 2.14 Cálculo de Financiamento
**Funcionalidades:**
- Permite simular condições de pagamento em tempo real
- Oferece transparência e agilidade na negociação
- Calcula parcelas, juros e prazos de forma personalizada
- Considera regras da instituição financeira
- Integração com taxas e condições de parceiros financeiros
- Apresentação clara e personalizada durante o atendimento
- Apoio à decisão de compra do cliente, sem precisar sair da conversa

### 2.15 Comparador de Preços para Avaliar Valor do Bem de Entrada
**Funcionalidades:**
- Avaliação do bem a ser dado como pagamento, ou parte do pagamento no valor total de compra
- Útil para negociações de carros, motos, imóveis
- Comparação de valores de mercado

### 2.16 Direcionamento para Atendentes por Ordem Programada
**Funcionalidades:**
- Deve ser definida uma lista de vendedores ordenada por um período pré-definido (em dias)
- O ciclo se repete quando chega no último vendedor
- Rotação da ordem dos vendedores para ter o máximo de oportunidades para cada um
- Distribuição equitativa de leads entre a equipe

### 2.17 Conversão e Transcrição de Mensagens
**Funcionalidades:**
- Processo automatizado para converter e transcrever diferentes formatos de mensagens recebidas
- **Áudio para texto:** Reconhecimento automático da fala para transformar mensagens de voz em texto legível e pesquisável
- **Texto para áudio:** Síntese de voz para transformar mensagens escritas em áudio, facilitando o consumo em diferentes contextos
- **Transcrição de PDFs:** Extração de texto de documentos PDF para consulta rápida e integração com fluxos automatizados
- **Identificação e transcrição de imagens:** Uso de OCR (reconhecimento óptico de caracteres) para extrair texto de imagens enviadas pelo cliente
- Garante acessibilidade, melhor entendimento e agilidade no atendimento

### 2.18 Configuração Vinculada ao Domínio do Cliente
**Funcionalidades:**
- Permite que o Evah Assistant funcione sob um subdomínio do cliente
- SSL e identidade visual personalizada
- Requer configuração de DNS (CNAME ou A record)
- Personalização completa da experiência do cliente

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
- Personalização de acordo com a atividade comercial do cliente (imobiliária, escritórios de serviços e consultoria diversas, venda de automóveis)

### 3.11 Agente Wiki de Empresa
**Funcionalidades:**
- Determina todas as informações da empresa
- Base de conhecimento integrada
- Respostas baseadas em informações institucionais

### 3.12 Agente Cálculo de Financiamento
**Funcionalidades:**
- Simulação de condições de pagamento em tempo real
- Cálculo de parcelas, juros e prazos
- Integração com taxas de parceiros financeiros
- Apresentação durante o atendimento

### 3.13 Agente Comparador de Preços
**Funcionalidades:**
- Avaliação do bem a ser dado como pagamento
- Comparação de valores de mercado
- Útil para negociações de carros, motos, imóveis

### 3.14 Agente Direcionamento para Atendentes
**Funcionalidades:**
- Lista de vendedores ordenada por período pré-definido
- Rotação automática de vendedores
- Distribuição equitativa de oportunidades
- Ciclo que se repete automaticamente

### 3.15 Agente Gateway de Pagamento (Detalhado)
**Funcionalidades:**
- Permite processar transações dentro do fluxo de atendimento
- Suporte a diferentes métodos de pagamento (cartão, Pix, boleto, etc.)
- Integração transparente com o CRM e ERP
- Confirmações em tempo real dentro do atendimento
- Segurança e conformidade com padrões de mercado
- Útil para vendas online ou presenciais
- Integração com múltiplos provedores (exemplo: PagSeguro)

### 3.16 Agente Assistente Corporativo
**Funcionalidades:**
- Assistente específico para o logista (empresa) para gerenciar áreas da empresa via agente
- Permite que a empresa gerencie suas próprias áreas através do assistente
- Automação de processos internos da empresa

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
   - Se áudio: transcreve para texto
   - Se imagem: (futuramente) extrai dados visuais
   - Se link: reconhece URL e categoriza como scraping
   - Encaminha texto para o orquestrador
3. **3_Orquestrador** - Detecta a intenção do cliente
   - Usa IA para identificar a intenção do cliente:
     - Saudação
     - Consulta de veículo/produto
     - Interesse com base em mídia
     - Agendamento
     - Registro ou atualização de lead
   - Retorna JSON com `agente_destino` e `mensagem`
4. **4_RoteadorDeAgentes** - Direciona para o agente correto
   - Usa switch para redirecionar ao fluxo certo com base em `agente_destino`
5. **Agentes Específicos:**
   - 5_AgenteBoasVindas - Envia mensagem de saudação personalizada
   - 6_AgenteConsultaVeiculos - Responde com produtos filtrados do banco
   - 7_AgenteWebScraping - Extrai dados de anúncios enviados e consulta banco
   - 8_AgenteAgendamento - Agenda horário com cliente
   - 9_AgenteCRM - Cria e atualiza lead no Odoo
   - 10_AgenteDesconhecido (Fallback) - Mensagem genérica ou encaminha para atendimento humano

**Organização dos Flows no N8N:**
- **Workflows Principais:**
  - `1_Main_EntradaMensagem`
  - `2_TratamentoMensagem`
  - `3_Orquestrador`
  - `4_RoteadorDeAgentes`
- **Subworkflows (Agentes):**
  - `Agentes/BoasVindas`
  - `Agentes/ConsultaVeiculos`
  - `Agentes/WebScraping`
  - `Agentes/Agendamento`
  - `Agentes/CRM`
  - `Agentes/Fallback`

### 4.3 Camadas da Arquitetura
1. **Camada de Entrada (Front-End de Comunicação)**
   - WhatsApp, Webchat (EVAH Chat)
   
2. **Camada de Inteligência**
   - EVAH Chat (Typebot) - Interface guiada
   - Evah Assistant - Assistente de IA
   
3. **Camada de Automações**
   - EVAH Conductor (n8n) - Executa lógicas de negócio
   - EVAH Connect - Ponte entre canais externos e módulos internos
   
4. **Camada de Backend e Gestão**
   - EVAH Omni (Chatwoot) - Atendentes humanos
   - EVAH ERP (Odoo) - Registro e gestão

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
- Tempo de resposta lento - clientes esperam respostas imediatas, mas sem chatbot dependem de disponibilidade humana
- Sobrecarga da equipe de atendimento - atendentes precisam lidar com perguntas repetitivas e simples
- Dificuldade em atender fora do horário comercial - sem IA, o atendimento pode parar à noite, fins de semana e feriados
- Alto custo com equipe de suporte - necessidade de contratar mais pessoas para suprir a demanda
- Baixa escalabilidade - quando o volume de clientes cresce, o atendimento humano pode não acompanhar
- 80% das perguntas são repetitivas e podem ser automatizadas (IBM)
- Até 70% das dúvidas poderiam ser automatizadas (Typebot)
- Agentes perdem 30% do tempo trocando de ferramentas (HBR)
- 60% do tempo gasto em tarefas repetitivas (McKinsey)

**Problemas de Experiência do Cliente:**
- Frustração do cliente - demora, falta de agilidade ou indisponibilidade desmotivam
- Perda de oportunidades de venda - clientes que não recebem resposta rápida podem desistir
  - 60% dos clientes desistem se não recebem resposta em até 1 hora (Zendesk)
  - Resposta rápida qualifica 7x mais leads (HBR)
  - Atraso de 5 minutos reduz 400% as chances de conversão (HBR)
  - 78% dos clientes compram da primeira empresa que responde
- Atendimento inconsistente - cada atendente pode responder de um jeito, sem padronização
- Falta de personalização - sem histórico integrado, o cliente precisa repetir informações várias vezes
  - 91% preferem marcas que oferecem personalização (Accenture)
  - 72% esperam que a empresa conheça histórico de interações (Salesforce)
  - 61% mudam de empresa após experiência ruim (Zendesk)
- Menor conveniência - clientes modernos preferem resolver rápido via WhatsApp, site ou redes sociais

**Problemas Estratégicos:**
- Menor competitividade - concorrentes que usam IA conseguem ser mais rápidos, baratos e eficazes
- Falta de dados sobre clientes - sem chatbot, a empresa perde registros automáticos de dúvidas, interesses e objeções
  - Sem CRM, 79% dos leads se perdem (HubSpot)
  - Empresas com métricas melhoram satisfação em 60% (McKinsey)
  - Empresas orientadas por dados crescem 23x mais rápido (McKinsey)
- Dificuldade em nutrir leads - sem automação, fica mais difícil transformar curiosos em compradores
- Imagem antiquada da empresa - ausência de inovação pode passar a impressão de empresa "parada no tempo"
- Menor fidelização - clientes que não têm suporte ágil podem migrar para concorrentes

**Estatísticas de Impacto:**
- 60% das empresas afirmam perder vendas por falhas no atendimento
- A falta de integração entre sistemas pode aumentar em até 30% o custo operacional
- Negócios que não utilizam automação gastam, em média, o dobro de tempo em tarefas repetitivas
- Perda de até 20% da receita por sistemas isolados (Forrester)
- 20-30% menos produtividade (Deloitte)
- Custos de TI aumentam 15-25% (IDC)
- Duplicidade de dados gera até 20% de perda anual

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
- Ajustar o Evah Assistant para apresentar o produto de forma intuitiva, com exemplos
- Criar base de prompts para abastecimento
- Configurar memória de contexto
- Organizar e finalizar os agentes do assistente
- Organizar o fluxo de atendimento guiado, para coleta de dados
- Definir apresentação oficial do Evah Assistant
- Explicar claramente o que o Evah Assistant faz
- Descrever as principais funcionalidades
- Criar lista de casos de uso

### 7.3 Funcionalidades Futuras
- Assistente específico para o logista (empresa) para gerenciar áreas da empresa via agente
- Integração com agenda de vendedores
- Melhorias em interpretação de imagens
- Expansão de integrações
- Implementar fallback com IA generativa
- Ajustar fluxo de memória contextual
- Testar com clientes reais
- Finalizar os workflows faltantes

### 7.4 Caso de Uso Específico: BiraBot (Bira Veículos)
**Contexto:**
Aiva (nome técnico), apresentado aos clientes como **BiraBot**, é um assistente virtual desenvolvido para realizar **atendimento automatizado em empresas de venda de veículos**.

**Foco:**
- Atendimento inicial com boas-vindas
- Entendimento do interesse do cliente
- Consulta de veículos disponíveis
- Registro e atualização de leads no CRM (Odoo)
- Agendamento de visitas
- Interpretação de mídia (áudio, imagem, link)
- Consulta baseada em links (web scraping)

**Objetivos Específicos:**
- Detectar e responder a saudações como "bom dia", "boa tarde", "olá", etc.
- Apresentar-se como BiraBot e explicar sua função
- Identificar tipo de veículo desejado
- Extrair informações como: marca/modelo, tipo (SUV, hatch, sedan...), ano mínimo e máximo, faixa de preço
- Integrar com agente que consulta banco de dados
- Apresentar resultados baseados nos filtros coletados
- Criar lead no início do atendimento
- Atualizar lead à medida que mais dados são fornecidos
- Perguntar disponibilidade do cliente
- Registrar data e hora sugerida
- (Futuramente) integrar com agenda de vendedores

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

## 🔄 9. INTEGRAÇÕES COM OUTROS MÓDULOS EVAH

### 9.1 EVAH ERP (Odoo)
- Integração nativa para consulta de produtos
- Registro de leads e oportunidades
- Consulta de estoque e pedidos
- Sincronização de dados

### 9.2 EVAH Omni (Chatwoot)
- Encaminhamento para atendimento humano
- Histórico centralizado
- Gestão de conversas

### 9.3 EVAH Conductor (n8n)
- Execução de automações
- Orquestração de fluxos
- Integração com sistemas externos

### 9.4 EVAH Connect
- Conexão com canais externos
- Integração com APIs de mercado
- Atua como ponte entre canais externos e os módulos internos do EVAH
- Conecta WhatsApp, Instagram, Facebook, Telegram e outros canais ao ecossistema

### 9.5 EVAH Maestro (n8n)
- Núcleo de automações inteligentes do ecossistema EVAH
- Permite criar, gerenciar e executar fluxos complexos
- Conecta múltiplos sistemas, canais e processos empresariais
- Design modular e escalável
- Automatiza operação com flexibilidade, agilidade e precisão
- Otimiza resultados e garante controle total

### 9.6 EVAH Code
- Serviços de desenvolvimento personalizados
- Criação de regras de negócio específicas para cada negócio
- Via APIs, banco de dados e webapp
- Criação de Componentes Exclusivos
- Integrações com Sistemas Legados ou Proprietários
- Extensão de Fluxos e Automações Complexas
- Personalização de Interface e Experiência Conversacional
- Criação de APIs Customizadas
- Suporte a Projetos Especiais e Provas de Conceito
- Gerenciamento de Ciclo de Vida do Código

---

## 📝 10. ROTEIRO DE LANDING PAGE

> **Objetivo:** Criar uma landing page persuasiva que destaque os pontos fortes do Evah Assistant e convença clientes potenciais a contratar o assistente virtual.

### 10.1 Estrutura da Landing Page

#### SEÇÃO 1: HERO / ABERTURA IMPACTANTE
**Título Principal (H1):**
```
Transforme Seu Atendimento em Vendas com Inteligência Artificial
```

**Subtítulo:**
```
O Evah Assistant é o assistente virtual que atende seus clientes 24/7, qualifica leads automaticamente e aumenta suas vendas enquanto você foca no que realmente importa.
```

**CTA Principal:**
- Botão: "Quero Transformar Meu Atendimento" / "Solicitar Demonstração Gratuita"
- Botão secundário: "Ver Como Funciona"

**Elemento Visual:**
- Vídeo de demonstração (30-60 segundos) ou animação do Evah Assistant em ação
- Estatísticas em destaque: "Atendimento 24/7", "Resposta em segundos", "Aumento de 40% em conversões"

#### SEÇÃO 2: O PROBLEMA (DORES DO CLIENTE)
**Título:**
```
Você está perdendo vendas enquanto dorme?
```

**Conteúdo:**
- **Dores principais:**
  - Clientes desistem porque não recebem resposta rápida
  - Equipe sobrecarregada com perguntas repetitivas
  - Leads se perdem sem follow-up adequado
  - Atendimento limitado a horário comercial
  - Dificuldade em escalar o atendimento

**Estatísticas de impacto:**
- "60% dos clientes desistem se não recebem resposta em até 1 hora"
- "80% das perguntas são repetitivas e podem ser automatizadas"
- "Empresas com chatbot convertem 7x mais leads"

**CTA de transição:**
- "Descubra como o Evah Assistant resolve isso"

#### SEÇÃO 3: A SOLUÇÃO (APRESENTAÇÃO DO Evah Assistant)
**Título:**
```
Evah Assistant: Seu Assistente Virtual Inteligente que Trabalha 24/7
```

**Subtítulo:**
```
Mais que um chatbot. Um assistente completo que entende, qualifica, vende e fideliza seus clientes.
```

**Diferenciais principais (3-4 cards):**

**Card 1: Inteligência Real**
- "Atendimento com IA avançada (ChatGPT, Gemini, Watson)"
- "Entende contexto, sentimentos e intenções do cliente"
- "Respostas personalizadas e naturais"

**Card 2: Multi-Canal**
- "Atende no WhatsApp, Instagram, Facebook, Telegram e WebChat"
- "Todas as conversas centralizadas em um só lugar"
- "Experiência consistente em todos os canais"

**Card 3: Automação Inteligente**
- "Qualifica e registra leads automaticamente no CRM"
- "Agenda compromissos no Google Calendar"
- "Consulta produtos, estoque e informações em tempo real"

**Card 4: Integração Total**
- "Conecta com seu ERP, CRM e sistemas existentes"
- "Gerencia arquivos no Google Drive"
- "Extrai dados de sites externos quando necessário"

**CTA:**
- "Quero ver o Evah Assistant em ação"

#### SEÇÃO 4: COMO FUNCIONA (DEMONSTRAÇÃO)
**Título:**
```
Veja o Evah Assistant em Ação
```

**Fluxo de demonstração (3-4 passos visuais):**

**Passo 1: Cliente chega**
- "Cliente envia mensagem via WhatsApp"
- "Evah Assistant responde instantaneamente com boas-vindas personalizadas"

**Passo 2: Inteligência em ação**
- "Evah Assistant identifica a intenção do cliente"
- "Consulta produtos no ERP em tempo real"
- "Apresenta opções personalizadas"

**Passo 3: Qualificação automática**
- "Coleta informações do cliente de forma natural"
- "Registra lead automaticamente no CRM"
- "Agenda visita ou reunião no Google Calendar"

**Passo 4: Conversão**
- "Cliente recebe todas as informações necessárias"
- "Lead qualificado é direcionado para o vendedor"
- "Venda é fechada com mais agilidade"

**Elemento Visual:**
- Screenshots ou vídeo animado mostrando o fluxo
- Timeline visual do processo

**CTA:**
- "Quero uma demonstração personalizada"

#### SEÇÃO 5: RECURSOS PRINCIPAIS (DESTAQUES)
**Título:**
```
Tudo que você precisa em um assistente inteligente
```

**Grid de recursos (organizado por categorias):**

##### 🤖 **Inteligência Artificial**
- **Atendimento com IA:** ChatGPT, Gemini, Watson - respostas contextuais e análise de sentimentos
- **Identificação de intenção:** Sabe quando o cliente quer comprar, tirar dúvidas ou apenas se apresentar
- **Contexto de conversação:** Lembra de tudo que foi dito, mantendo a conversa coerente e personalizada

##### 📱 **Multi-Canal**
- **WhatsApp (Evolution API):** Rápido e flexível para começar
- **WhatsApp (Meta Oficial):** Conformidade total e recursos exclusivos
- **Instagram:** Atende DMs e interações
- **Facebook Messenger:** Integração nativa
- **Telegram:** API gratuita e poderosa
- **WebChat:** Widget no seu site

##### 🔄 **Automações Inteligentes**
- **Gestão de Leads no CRM:** Cria, atualiza e promove leads automaticamente
- **Agendamentos:** Sincroniza com Google Calendar
- **Gestão de Arquivos:** Upload, download e organização no Google Drive
- **Web Scraping:** Extrai dados de sites em tempo real

##### 🎯 **Integração com Sistemas**
- **Consulta de Produtos:** Verifica estoque e detalhes no ERP
- **Exibição de Fotos:** Mostra imagens dos produtos
- **Consulta FIPE:** Valores atualizados de veículos
- **Processamento Multimídia:** Recebe áudios e analisa imagens

##### 👥 **Atendimento Humanizado**
- **Atendimento Guiado:** Fluxos personalizados no Typebot
- **Redirecionamento Inteligente:** Transfere para humano quando necessário
- **Análise de Sentimentos:** Identifica quando o cliente precisa de atenção especial

**CTA:**
- "Quero conhecer todos os recursos"

#### SEÇÃO 6: BENEFÍCIOS E RESULTADOS
**Título:**
```
Resultados Reais para Seu Negócio
```

**Benefícios em números (cards com estatísticas):**

**Card 1: Atendimento 24/7**
- "Nunca perca uma venda por falta de resposta"
- "Atenda clientes mesmo fora do horário comercial"
- "Aumente sua disponibilidade sem aumentar custos"

**Card 2: Qualificação Automática**
- "Leads qualificados automaticamente no CRM"
- "Reduza tempo de qualificação manual em 80%"
- "Aumente a taxa de conversão de leads"

**Card 3: Escalabilidade**
- "Atenda múltiplos clientes simultaneamente"
- "Sem limites de atendimentos por dia"
- "Cresça sem precisar contratar mais atendentes"

**Card 4: Redução de Custos**
- "Reduza custos com equipe de atendimento"
- "Automatize 80% das perguntas repetitivas"
- "ROI positivo em menos de 3 meses"

**Card 5: Experiência do Cliente**
- "Respostas instantâneas e personalizadas"
- "Atendimento consistente em todos os canais"
- "Cliente nunca precisa repetir informações"

**Card 6: Dados e Insights**
- "Histórico completo de todas as interações"
- "Relatórios de desempenho e conversão"
- "Dados para tomar decisões estratégicas"

**CTA:**
- "Quero esses resultados no meu negócio"

#### SEÇÃO 7: CASOS DE SUCESSO / DEPOIMENTOS
**Título:**
```
Empresas que já transformaram seu atendimento com o Evah Assistant
```

**Case 1: Bira Veículos**
- "Aumento de 40% em agendamentos de visitas"
- "Redução de 60% no tempo de resposta"
- "Leads qualificados automaticamente no CRM"

**Depoimento:**
> "O Evah Assistant revolucionou nosso atendimento. Agora atendemos 24/7 e nunca perdemos um lead. A integração com nosso sistema foi perfeita." - [Nome do Cliente]

**Case 2: [Outro cliente]**
- Métricas e resultados específicos
- Depoimento em vídeo ou texto

**Elemento Visual:**
- Logos dos clientes
- Screenshots de resultados
- Vídeos de depoimentos (se disponível)

**CTA:**
- "Quero ser o próximo case de sucesso"

#### SEÇÃO 8: DIFERENCIAIS COMPETITIVOS
**Título:**
```
Por que escolher o Evah Assistant?
```

**Comparativo (tabela ou cards):**

**Diferencial 1: Inteligência Real**
- "Não é apenas um chatbot com respostas prontas"
- "IA avançada que entende contexto e intenções"
- "Aprende e se adapta ao seu negócio"

**Diferencial 2: Integração Completa**
- "Conecta com seus sistemas existentes (ERP, CRM)"
- "Não precisa trocar tudo que você já tem"
- "Funciona com o que você já usa"

**Diferencial 3: Multi-Canal Unificado**
- "Um assistente para todos os canais"
- "Histórico centralizado"
- "Experiência consistente"

**Diferencial 4: Personalização Total**
- "Adaptado ao seu negócio e segmento"
- "Fluxos personalizados para suas necessidades"
- "Linguagem e tom da sua marca"

**Diferencial 5: Suporte e Evolução**
- "Equipe técnica especializada"
- "Atualizações constantes"
- "Suporte contínuo"

**CTA:**
- "Quero conhecer os diferenciais"

#### SEÇÃO 9: COMO COMEÇAR (PROCESSO)
**Título:**
```
Comece a transformar seu atendimento em 3 passos simples
```

**Passo 1: Demonstração**
- "Agende uma demonstração gratuita"
- "Veja o Evah Assistant funcionando com seus dados reais"
- "Entenda como se adapta ao seu negócio"

**Passo 2: Personalização**
- "Nossa equipe configura o Evah Assistant para seu negócio"
- "Integramos com seus sistemas existentes"
- "Treinamos sua equipe"

**Passo 3: Lançamento**
- "Evah Assistant começa a atender seus clientes"
- "Monitoramento e ajustes contínuos"
- "Suporte dedicado"

**Timeline:**
- "De 7 a 15 dias para estar funcionando"

**CTA:**
- "Quero começar agora"

#### SEÇÃO 10: PLANOS E INVESTIMENTO
**Título:**
```
Planos que se adaptam ao seu negócio
```

**Estrutura de planos (3 opções):**

**Plano Básico:**
- Ideal para pequenas empresas
- Recursos essenciais
- Até X atendimentos/mês
- Preço: R$ X/mês

**Plano Intermediário:**
- Ideal para empresas em crescimento
- Recursos completos
- Até X atendimentos/mês
- Preço: R$ X/mês
- **Mais popular**

**Plano Avançado:**
- Ideal para grandes empresas
- Recursos ilimitados
- Atendimentos ilimitados
- Preço: R$ X/mês

**O que está incluído em todos os planos:**
- ✅ Atendimento 24/7
- ✅ Multi-canal (WhatsApp, Instagram, etc.)
- ✅ Integração com CRM
- ✅ Suporte técnico
- ✅ Atualizações

**CTA:**
- "Quero ver os planos detalhados"
- "Falar com um especialista"

#### SEÇÃO 11: PERGUNTAS FREQUENTES (FAQ)
**Título:**
```
Dúvidas Frequentes
```

**Perguntas principais:**

1. **Quanto tempo leva para implementar o Evah Assistant?**
   - Resposta sobre o processo e timeline

2. **Preciso ter algum sistema específico?**
   - Resposta sobre integrações e compatibilidade

3. **O Evah Assistant substitui minha equipe de atendimento?**
   - Resposta sobre complementaridade e redirecionamento

4. **Como funciona a integração com meu CRM/ERP?**
   - Resposta sobre APIs e conectores

5. **Posso personalizar o Evah Assistant para meu negócio?**
   - Resposta sobre customização e adaptação

6. **Quais são os custos adicionais?**
   - Resposta sobre custos de APIs e infraestrutura

7. **O Evah Assistant funciona em outros idiomas?**
   - Resposta sobre suporte multilíngue

8. **Como é o suporte técnico?**
   - Resposta sobre suporte e SLA

#### SEÇÃO 12: CTA FINAL / FORMULÁRIO DE CONTATO
**Título:**
```
Pronto para transformar seu atendimento?
```

**Subtítulo:**
```
Solicite uma demonstração gratuita e veja como o Evah Assistant pode aumentar suas vendas
```

**Formulário de contato:**
- Nome completo
- E-mail
- Telefone/WhatsApp
- Nome da empresa
- Segmento de atuação
- Quantidade de atendimentos/mês (estimativa)
- Mensagem (opcional)

**Benefícios do formulário:**
- "Demonstração gratuita"
- "Sem compromisso"
- "Resposta em até 24 horas"

**Informações de contato alternativas:**
- WhatsApp: [número]
- E-mail: [email]
- Telefone: [telefone]

**Garantias/Prova social:**
- "Mais de X empresas já confiam no Evah Assistant"
- "Satisfação garantida"
- "Suporte dedicado"

#### SEÇÃO 13: RODAPÉ
**Elementos:**
- Logo da Dobem Tecnologia
- Links importantes:
  - Sobre nós
  - Cases de sucesso
  - Blog/Recursos
  - Contato
- Redes sociais
- Política de privacidade
- Termos de uso
- Copyright

### 10.2 Elementos Visuais Recomendados

**Imagens e Vídeos:**
- Vídeo de demonstração do Evah Assistant (30-60s)
- Screenshots do assistente em ação
- Infográficos dos benefícios
- Ícones para cada funcionalidade
- Animações sutis de interação

**Cores e Estilo:**
- Paleta profissional e moderna
- Destaque para CTAs (botões de ação)
- Tipografia clara e legível
- Espaçamento generoso
- Design responsivo (mobile-first)

### 10.3 Métricas de Conversão

**Elementos para rastrear:**
- Cliques no CTA principal
- Visualizações do vídeo
- Preenchimentos do formulário
- Tempo na página
- Taxa de rejeição
- Scroll depth (até onde o usuário rola)

**Testes A/B sugeridos:**
- Diferentes títulos hero
- Cores dos botões CTA
- Posicionamento do formulário
- Textos de benefícios
- Ordem das seções

### 10.4 Otimizações SEO

**Palavras-chave principais:**
- Assistente virtual inteligente
- Chatbot com IA
- Atendimento automatizado
- Qualificação de leads automática
- Assistente virtual WhatsApp

**Meta tags:**
- Título: "Evah Assistant - Assistente Virtual Inteligente que Aumenta Suas Vendas"
- Descrição: "Transforme seu atendimento com IA. Atendimento 24/7, qualificação automática de leads e integração completa. Solicite demonstração gratuita."

### 10.5 Notas de Implementação

**Prioridades para MVP:**
1. Hero section com CTA forte
2. Seção de problemas/dores
3. Apresentação do Evah Assistant
4. Recursos principais
5. Formulário de contato

**Melhorias futuras:**
- Calculadora de ROI
- Chatbot de demonstração na própria página
- Comparativo com concorrentes
- Blog com cases detalhados
- Área de login para clientes

---

## 📝 11. NOTAS E OBSERVAÇÕES

### 11.1 Nomenclatura
- Há variação entre "Evah Assistant" e "EVAH" nos documentos
- "Evah Assistant" parece ser o nome técnico
- "EVAH" parece ser o nome comercial/apresentação
- Pode ter nomes customizados por cliente (ex: BiraBot)

### 11.2 Adaptabilidade
- O Evah Assistant deve ser capaz de se adaptar à realidade do negócio do cliente
- Personalização por segmento e contexto
- Flexibilidade para diferentes casos de uso

### 11.3 Foco no MVP
- Priorizar funcionalidades essenciais
- Garantir estabilidade e confiabilidade
- Focar em casos de uso principais
- Demonstrar valor imediato
- Nome e identidade clara (`EVAH` como framework, `Evah Assistant` como exemplo aplicado)
- Demonstração funcional que mostre valor imediato
- Capacidade de modularização (usar só o que o cliente precisa)
- Resolução de problemas reais

### 11.4 Objetivo do Projeto
Entregar uma **solução vendável, funcional e escalável** nas mãos do vendedor. O framework EVAH permite montar soluções sob medida para resolver as dores reais do processo comercial.

### 11.5 Posicionamento Estratégico
O EVAH é pensado para **crescer com o cliente**: Empresas podem começar com um módulo como o `Evah Assistant` e, conforme amadurecem, escalar para soluções mais completas. Isso reduz barreiras de entrada, acelera a implementação e aumenta a retenção no longo prazo.

### 11.6 Identidade Visual
- Logo: "Evah Assistant - Assistente Inteligente de vendas"
- Apresentação pode variar conforme cliente (ex: BiraBot para Bira Veículos)

### 11.7 Processo de Implantação
**Etapas Principais:**
1. **API Integração com WhatsApp:**
   - Criar uma instância na AWS para implantar a EvolutionAPI
   - Configurar a instância (docker, swarm, portainer, traefik...)
   - Implantar a Stack via yml
   - Criar e registrar um subdomínio único para disponibilizar a API
   - Opção: Evolution API (gratuita) ou API oficial da Meta (exige número verificado + cobrança por conversa)

2. **Integrações com Outros Canais:**
   - API Integração com Instagram
   - API Integração com Telegram (Gratuito)
   - API Integração com Facebook (Gratuito)
   - API Integração com WebChat

3. **Configuração e Personalização:**
   - Configuração vinculada ao domínio do cliente
   - Integração com API de inteligência Artificial (Custos variáveis)
   - Integração com Google calendar
   - Integração com Google Drive
   - Implantação do Typebot (Atendimento guiado)
   - Integração com EVAH ERP para consulta de produtos
   - Desenvolvimento de fluxos de negócio
   - Personalização do Assistente

4. **Conversão e Transcrição:**
   - Implementar processo automatizado para converter e transcrever diferentes formatos de mensagens

### 11.8 Custos e Preços (Referência)
**Componentes Principais:**
- Typebot (Hospedagem automática): R$ 100,00
- Typebot (Widget em sites): R$ 100,00
- Agentes IA (vários): R$ 0,02 por uso (OpenAI)
- Atendimento WhatsApp (Evolution API): R$ 100,00
- Atendimento WhatsApp (Meta Oficial): R$ 0,03 por conversa
- Atendimento Instagram: R$ 0,03 por conversa
- Atendimento Facebook Messenger: R$ 0,03 por conversa
- Atendimento Telegram: R$ 100,00
- Atendimento WebChat: R$ 82,20
- Assistentes de IA: R$ 500,00
- Hospedagem Onpremise: R$ 82,20 por serviço
- Banco de dados (RDS): R$ 100,00
- Gateway de Pagamento: R$ 3,50 (exemplo: PagSeguro)

**Nota:** Valores são referências e podem variar conforme configuração e uso.

---

**Última atualização:** 2025  
**Fonte:** Consolidação de múltiplos arquivos do projeto

