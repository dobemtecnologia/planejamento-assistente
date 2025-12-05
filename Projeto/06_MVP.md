# 🛠️ BACKLOG DO MVP - EVAH Platform

> **Documento Técnico de Desenvolvimento**
> **Objetivo:** Entregar a versão 1.0 vendável (Foco: Concessionárias/Varejo - Case Bira)
> **Stack:** n8n, Typebot, Evolution API, OpenAI, Odoo, Chatwoot.
> **Versão:** 1.0 - Definição Inicial

---

## 📋 DEFINIÇÃO DE DONE (DoD) DO MVP

Para considerar o MVP pronto para venda, o sistema deve obrigatoriamente:

1.  **Receber mensagens** via WhatsApp (Evolution API) em tempo real.
2.  **Triar a intenção** do usuário usando IA (OpenAI) dentro do n8n.
3.  **Executar duas ações reais:**
    * Consultar Tabela/Preço.
    * Agendar Reunião no Google Calendar.
4.  **Registrar o lead** automaticamente no CRM (Odoo) com dados básicos.
5.  **Transbordar para humano** no Chatwoot caso a IA falhe ou o cliente solicite.

---

## 🧩 ÉPICO 1: INFRAESTRUTURA & AMBIENTE (Foundation)
*Configuração do "terreno" onde a EVAH vai rodar.*

| ID | História / Tarefa | Critérios de Aceite (Técnico) | Prioridade |
| :--- | :--- | :--- | :--- |
| **INF-01** | **Setup do Cluster Docker** | - Servidor VPS/AWS provisionado.<br>- Docker Swarm e Portainer instalados e seguros.<br>- Traefik configurado como Proxy Reverso com SSL (Let's Encrypt). | **Alta** |
| **INF-02** | **Deploy do Stack Core** | - Containers rodando: n8n, Typebot, Evolution API, Chatwoot, PostgreSQL, Redis.<br>- Comunicação interna entre containers validada via rede Docker. | **Alta** |
| **INF-03** | **Instalação do Odoo (ERP)** | - Odoo Community instalado.<br>- Módulos básicos ativos: CRM, Vendas, Calendário.<br>- Acesso administrativo configurado e testado. | **Alta** |
| **INF-04** | **Monitoramento Básico** | - Uptime Kuma configurado monitorando os endpoints das APIs.<br>- Alerta de queda configurado (email ou Telegram). | Média |

---

## 🧩 ÉPICO 2: CANAIS & CONECTIVIDADE (The Mouth)
*Garantir que a EVAH "ouça" e "fale" com o mundo.*

| ID | História / Tarefa | Critérios de Aceite (Técnico) | Prioridade |
| :--- | :--- | :--- | :--- |
| **CON-01** | **Conexão WhatsApp (Evolution API)** | - Instância criada na Evolution API.<br>- QR Code lido e sessão com status "Connected".<br>- Webhook configurado apontando para o n8n (Workflow de Entrada). | **Alta** |
| **CON-02** | **Integração Chatwoot (Transbordo)** | - Caixa de entrada criada no Chatwoot.<br>- Webhook do Chatwoot conectado ao n8n (para ouvir respostas do humano).<br>- Agentes humanos cadastrados com acesso. | **Alta** |
| **CON-03** | **Roteador de Mensagens (n8n)** | - Workflow "Main_Router" criado.<br>- Lógica: Se mensagem nova -> Envia para IA.<br>- Lógica: Se atendimento humano aberto (status open) -> Não interfere (pausa IA). | **Alta** |

---

## 🧩 ÉPICO 3: INTELIGÊNCIA & CÉREBRO (The Brain)
*A lógica que entende o cliente e decide o que fazer.*

| ID | História / Tarefa | Critérios de Aceite (Técnico) | Prioridade |
| :--- | :--- | :--- | :--- |
| **INT-01** | **Agente de Triagem (OpenAI)** | - Nó OpenAI no n8n configurado (GPT-4o-mini ou GPT-3.5-turbo para rapidez/custo).<br>- System Prompt definido: "Você é a Evah, assistente da empresa X...".<br>- Capacidade de classificar intenção: *Dúvida, Compra, Agendamento, Falar com Humano*. | **Alta** |
| **INT-02** | **Memória de Conversa (Contexto)** | - Uso do Zep ou Buffer no Postgres/Redis para manter histórico das últimas 10 mensagens.<br>- IA responde considerando o que foi dito antes (ex: lembra o nome do cliente durante a sessão). | **Alta** |
| **INT-03** | **Tratamento de Áudio (Whisper)** | - Se mensagem = áudio -> Enviar para Whisper API -> Converter em texto -> Passar para o fluxo normal da IA.<br>- Resposta da IA deve ser em texto (nesta fase). | **Alta** |

---

## 🧩 ÉPICO 4: AGENTES DE AÇÃO "KILLER" (The Muscle)
*O diferencial competitivo: Vertical AI que executa.*

| ID | História / Tarefa | Critérios de Aceite (Técnico) | Prioridade |
| :--- | :--- | :--- | :--- |
| **ACT-01** | **Agente de Agendamento (Google Calendar)** | - Autenticação OAuth2 com Google Calendar configurada no n8n.<br>- Fluxo: Cliente pede horário -> IA consulta slots livres -> IA oferece opções -> Cliente escolhe -> IA cria evento na agenda. | **Alta** |
| **ACT-02** | **Agente de Consulta (Tabela/Scraper)** | - **Opção A (MVP Rápido):** Consulta em Tabela Google Sheets ou Banco de Dados interno (ex: Tabela de Preços).<br>- **Opção B (Case Bira):** Nó de Scraper (n8n) que consulta FIPE ou site específico.<br>- IA retorna o valor exato para o cliente no chat. | **Alta** |
| **ACT-03** | **Agente de Qualificação (Perguntas)** | - Fluxo (pode ser Typebot para mais rigor) que coleta dados estruturados: Nome, Email, Interesse.<br>- Validação básica (ex: se email tem "@"). | Média |

---

## 🧩 ÉPICO 5: GESTÃO & CRM (The Memory)
*Onde o valor do negócio é armazenado.*

| ID | História / Tarefa | Critérios de Aceite (Técnico) | Prioridade |
| :--- | :--- | :--- | :--- |
| **CRM-01** | **Criação Automática de Lead** | - Quando IA identifica "Interesse de Compra" -> Criar Lead no Odoo CRM via API.<br>- Campos obrigatórios: Nome, Telefone (WhatsApp), Origem. | **Alta** |
| **CRM-02** | **Atualização de Lead (Log)** | - Salvar resumo da conversa ou nota no card do Lead no Odoo.<br>- Permitir que o vendedor veja o contexto do que foi conversado. | Média |
| **CRM-03** | **Notificação de Venda** | - Se Lead for classificado como "Quente" (High Ticket) -> Enviar alerta no grupo de WhatsApp da equipe comercial. | Baixa |

---

## 📅 SUGESTÃO DE SPRINTS (CRONOGRAMA TÉCNICO)

### Sprint 1: Fundação (Semana 1)
* **Foco:** Infraestrutura e "Hello World".
* **Entregável:** Servidor de pé, WhatsApp conectado, respondendo "Olá" automático.
* *Tarefas:* INF-01, INF-02, CON-01.

### Sprint 2: O Cérebro (Semana 2)
* **Foco:** Inteligência e CRM.
* **Entregável:** IA conversando com contexto e salvando Leads no Odoo.
* *Tarefas:* INT-01, INT-02, CRM-01, CON-02, CON-03.

### Sprint 3: A Execução (Semana 3)
* **Foco:** Agendamento e Áudio.
* **Entregável:** Cliente consegue agendar reunião e mandar áudio.
* *Tarefas:* ACT-01, INT-03, INF-03.

### Sprint 4: Polimento e Go-Live (Semana 4)
* **Foco:** Testes de carga, Consulta de Preço e Refinamento de Prompts.
* **Entregável:** Produto pronto para o primeiro cliente (Bira/Piloto).
* *Tarefas:* ACT-02, Ajustes finais de fluxo.

---

### 💡 Nota Técnica para o CTO/Dev
> *A arquitetura deve priorizar o **n8n** como orquestrador central. Evite hard-code (código puro) dentro da aplicação principal. Use o n8n para lógica de negócios, pois isso permite que a equipe de operações ajuste fluxos sem precisar de deploy de código.*