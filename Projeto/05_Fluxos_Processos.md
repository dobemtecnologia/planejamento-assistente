# 🔄 FLUXOS E PROCESSOS - EVAH

## 📋 Índice
- [Arquitetura Geral](#arquitetura-geral)
- [Workflows e Automações](#workflows-e-automações)
- [Integrações Técnicas](#integrações-técnicas)
- [Infraestrutura](#infraestrutura)
- [Processos Operacionais](#processos-operacionais)

---

## 🏗️ Arquitetura Geral

### Visão Geral do Ecossistema EVAH

```
EVAH - Ecossistema de Valor Automatizado para Humanos
│
├── ERP (Sistema de gestão)
├── MAESTRO (Automação - n8n)
├── EVAH (Assistente Virtual com IA)
├── OMNIN (Atendimento omnichannel - Chatwoot)
└── Inputs (Entradas de dados)
```

**Conclusão Estratégica:**
A Dobem não vende produtos isolados, mas um **ecossistema integrado** que resolve problemas end-to-end do cliente.

### Arquitetura Modular de Agentes

**Estrutura Identificada:**
```
Assistente
├── Assistente Venda (Especializado)
├── Orquestrador (n8n) - Coordenação central
├── Agente A (Especializado)
├── Agente B (Especializado)
├── Agente C (Especializado)
└── Agente de Negócio (Específico da empresa)
    └── Aplica regras de negócio aqui ← DIFERENCIAL
```

**Análise:**
- **Modularidade:** Permite escalar e personalizar por cliente
- **Orquestração Central:** n8n como cérebro que coordena tudo
- **Agente de Negócio:** Onde a mágica acontece - personalização profunda
- **Especialização:** Cada agente faz uma coisa muito bem

**Vantagem Competitiva:**
Esta arquitetura permite que a Dobem crie soluções únicas para cada cliente, mantendo a base tecnológica reutilizável.

### Arquitetura em Camadas

A estrutura técnica do EVAH pode ser organizada em quatro camadas funcionais:

1. **Camada de Entrada (Front-End de Comunicação)**
   - WhatsApp, Webchat (EVAH Chat)
   - Pontos de contato onde o cliente inicia a interação com a empresa

2. **Camada de Inteligência**
   - **EVAH Chat** - Interface guiada que conduz fluxos automatizados
   - **EVAH Evah Assistant** - Assistente de IA para atendimento natural e vendas automatizadas

3. **Camada de Automações**
   - **EVAH Conductor (n8n)** - Executa lógicas de negócio, orquestra integrações e automatiza tarefas
   - **EVAH Connect** - Atua como ponte entre canais externos e os módulos internos do EVAH

4. **Camada de Backend e Gestão**
   - **EVAH Omni (Chatwoot)** - Atendentes humanos assumem o controle quando necessário
   - **EVAH ERP (Odoo)** - Registra dados, gerencia operações comerciais, administrativas e financeiras

### Benefícios da Arquitetura Modular

- Flexibilidade para adaptar regras e processos por cliente
- Integração com ferramentas modernas via APIs abertas
- Capacidade de automação total ou parcial de atendimentos
- Centralização de dados em um núcleo de gestão confiável
- Substituição ou evolução de módulos sem comprometer o ecossistema

## ⚡ Workflows e Automações

### Fluxo de Processamento de Mensagens

**Fluxo Identificado:**
```
Mensagem recebida
    ↓
Identificar tipo de mensagem
    ├─ Texto → Repassa direto
    ├─ Áudio → Converter para texto
    └─ Imagem/Vídeo → Extrair dados visuais → Converter para texto
        └─ Erro → Mensagem educativa ao usuário
```

**Análise:**
- **Robustez:** Trata todos os tipos de entrada
- **UX:** Mensagens de erro educativas
- **Inteligência:** Extrai dados de imagens (OCR, visão computacional)

### Fluxo de Captura e Qualificação de Lead

**Fluxo Identificado:**
```
Mensagem recebida
    ↓
Identificar origem do Lead (WhatsApp, Instagram, etc.)
    ↓
Salvar Lead no CRM (Odoo)
    ↓
Verificar se contato já existe
    ↓
Atribuir lead?
    ├─ SIM → Qualificar no CRM
    └─ NÃO → Criar oportunidade no Odoo
```

**Análise:**
- **Rastreamento:** Origem do lead é sempre registrada
- **Inteligência:** Evita duplicação de contatos
- **Automação:** Criação automática de oportunidades
- **Integração:** Direta com CRM

### Fluxo de Agendamento

**Fluxo Identificado:**
```
Agente Orquestrador
    ↓
Agente verifica disponibilidade (Google Calendar)
    ↓
Agente cria evento
    ↓
Enviar notificação (email, SMS)
```

**Análise:**
- **Automação completa:** Do pedido à confirmação
- **Integração:** Google Calendar nativo
- **Notificações:** Múltiplos canais

### Fluxos Operacionais Completos - Caso Bira Veículos

#### QUADRO 1: Plataforma (Cegonha) - Preparação de Veículos

**Processo Mapeado:**
- Revisão mecânica
- Pintura veicular
- Martelinho de ouro
- Lavagem
- Polimento
- Entrada no sistema (Autoconfiguração)

**Insight de Negócio:**
A Dobem não apenas automatiza atendimento, mas **mapeia processos completos** do cliente para criar automações end-to-end.

#### QUADRO 2: Compra - Pré-compra, Avaliação e Precificação

**Fluxo Detalhado:**
1. **Solicitação de avaliação:**
   - Verificação: Tem chave reserva?
   - Coleta de dados: Nome, telefone, CRLV, manual e chave
   - Lançamento no custo do carro
   - Identificação dos custos do veículo

2. **Tipo de operação:**
   - Carro novo: SIM → Troca ou Compra

**Insight de Negócio:**
O sistema precisa entender **lógica de negócio complexa** do cliente, não apenas responder perguntas.

#### QUADRO 3: Captura de Mídia, Anúncios, Leads e Pré-atendimento

**Processos:**
- Captura de mídia do carro
- Anúncios
- Captura de Lead
- Pré-atendimento

**Insight de Negócio:**
A Dobem automatiza desde a **captura inicial** até o **pré-atendimento**, criando um funil completo.

#### QUADRO 4: Venda na Loja - Processo Completo de Venda

**Fluxo Completo Identificado:**

**Fase 1: Análise e Simulação**
- Faz análise em todos os bancos
- Simulação de taxa
- Avaliar potencial de financiamento do cliente

**Fase 2: Negociação**
- Atendimento
- Somente em 5 ou mais (regra de negócio)
- Verifica se tem carro na troca
- Avalia o valor do carro

**Fase 3: Financiamento Aprovado**
- **SIM:**
  - Realiza pagamento da transferência
  - Assina recibo
  - Assina doc de procuração para funcionamento
  - Assina checklist de entrega
  - Realiza entrega do carro
- **NÃO:**
  - Verifica se caiu na conta
  - Transferência da entrada (Priscila - pessoa específica)
  - Recebimento dos docs
  - Docs pendentes

**Análise Estratégica:**
Este fluxo mostra que a Dobem não está apenas criando um chatbot, mas **automatizando processos complexos de negócio** que envolvem:
- Múltiplas etapas
- Decisões condicionais
- Integração com sistemas externos (bancos)
- Gestão de documentos
- Rastreamento de status
- Pessoas específicas (Priscila)

## 🔗 Integrações Técnicas

### EVAH Connect - Módulo de Integração

O **EVAH Connect** conecta canais externos, como WhatsApp, e sistemas externos ao ecossistema **EVAH**.

**Funcionalidades:**
- Integração com WhatsApp (Evolution API ou Meta Official)
- Integração com Instagram, Facebook Messenger, Telegram
- Integração com WebChat
- Conectores para sistemas externos
- APIs padronizadas para extensões

### EVAH Conductor (n8n) - Orquestrador de Automações

O **EVAH Conductor** é o núcleo de automações do ecossistema **EVAH**, utilizando n8n para criar, gerenciar e executar fluxos complexos.

**Funcionalidades Principais:**

* **Construção Visual de Workflows**  
  Ambiente intuitivo para montar fluxos de automação através de uma interface drag-and-drop, sem necessidade de programação avançada.

* **Integração Nativa com Sistemas e APIs**  
  Conexão direta com ERP (como Odoo), CRM, bancos de dados, ferramentas de comunicação (WhatsApp via EVAH Connect), e serviços externos via APIs REST e Webhooks.

* **Processamento e Transformação de Dados**  
  Capacidade de manipular, transformar e validar dados recebidos antes de enviá-los para outros sistemas, assegurando integridade e conformidade.

* **Automação Condicional Avançada**  
  Execução de ações baseadas em regras condicionais complexas, incluindo verificações de múltiplos parâmetros, decisões ramificadas e loops.

* **Gerenciamento de Tarefas Programadas e Eventos**  
  Agendamento de execuções periódicas ou disparo de fluxos em resposta a eventos específicos, como recebimento de mensagens, atualizações em sistemas ou triggers personalizados.

* **Suporte a Automação de Processos de Atendimento**  
  Automatiza ações típicas do atendimento, como envio de notificações, follow-ups, criação e atualização de tickets, e transferências entre canais e agentes.

* **Monitoramento em Tempo Real e Alertas**  
  Dashboard para acompanhar o status das automações, com alertas configuráveis para falhas, lentidão ou inconsistências, facilitando a manutenção proativa.

* **Escalabilidade e Redundância**  
  Arquitetura preparada para suportar crescimento da operação, com possibilidade de distribuir cargas e executar múltiplos workflows simultaneamente.

* **Logs e Auditoria Detalhada**  
  Registro completo de todas as execuções, incluindo dados de entrada, saída, tempo de processamento e erros, essencial para compliance e análise de performance.

* **Suporte a Autenticação e Segurança**  
  Integra mecanismos de autenticação para APIs e serviços, garantindo comunicação segura entre sistemas.

* **Recuperação e Retentativa Automática**  
  Possui capacidade de retry automático em casos de falhas temporárias, minimizando interrupções no fluxo operacional.

* **Conectividade com Serviços de Mensageria e Cloud**  
  Integração com plataformas como AWS, Google Cloud, Azure, serviços de e-mail, SMS e notificações push.

* **Automação Híbrida com Intervenção Humana**  
  Permite pausar fluxos e encaminhar casos para atendentes humanos, integrando perfeitamente o trabalho da IA e dos operadores.

* **Versionamento e Gestão de Fluxos**  
  Controle de versões para os workflows, possibilitando rollback e gerenciamento seguro das automações em produção.

* **Extensibilidade via Custom Nodes**  
  Suporte à criação de nós personalizados para atender regras específicas ou conectar sistemas proprietários do cliente.

* **Suporte Omnichannel**  
  Gerencia fluxos que envolvem diferentes canais simultaneamente, garantindo que a operação mantenha consistência e integração total.

## 🖥️ Infraestrutura

### Stack Tecnológico

**Infraestrutura:**
- AWS EC2 (Large)
- Docker Swarm ou Kubernetes
- Traefik (Proxy reverso)
- Portainer (Gerenciamento)
- REDIS (Cache e filas)
- PostgreSQL (RDS)

**Conclusão:**
Stack moderna, escalável e baseada em containers. Permite:
- Deploy rápido
- Escalabilidade horizontal
- Isolamento de recursos
- Facilidade de manutenção

### Modelos de Hospedagem

#### Modelo 1: Servidor Dedicado (Onpremisse)
- Cada empresa tem seu próprio servidor
- Isolamento total
- Maior controle e segurança
- Custo mais alto

#### Modelo 2: Servidor Compartilhado (SaaS)
- Múltiplas empresas compartilham infraestrutura
- Odoo compartilhado
- Modelo multi-tenant
- Custo mais baixo
- Escalabilidade

**Análise Estratégica:**
A Dobem oferece **flexibilidade** ao cliente:
- Pequenas empresas: SaaS (menor custo)
- Grandes empresas: Onpremisse (maior controle)
- Permite migração conforme crescimento

### Infraestrutura Cloud (AWS)

- **Servidores AWS** - Infraestrutura principal na nuvem
- **AWS ECS (Elastic Container Service)** - Orquestração de containers
  - Cluster: `dobemtech-cluster`
  - Task Family: `dobemtech-task`
  - Log Group: `/ecs/dobemtech`
- **Monitoramento de custos e desempenho** - Acompanhamento contínuo dos serviços AWS
- **Lambdas AWS** - Email de disparo
- **Repositório para stacks** - Gerenciamento de configurações de infraestrutura
- **Terraform** - Infraestrutura como código

### Segurança e Monitoramento

- Armazenamento seguro de credenciais (cofre de senhas adequado)
- Centralização de emails de acordo com os Alias em todas as aplicações
- Uptime Kuma para monitoramento de APIs, sites, etc.
- Monitoramento contínuo de custos e desempenho AWS
- APIs com autenticação e autorização
- Dados criptografados em trânsito e em repouso
- Conformidade com LGPD

## 📋 Processos Operacionais

### Processo de Onboarding

**Etapas:**
1. Análise de necessidades do cliente
2. Mapeamento de processos e integrações
3. Configuração e personalização do assistente
4. Treinamento da equipe
5. Timeline: 7-15 dias (setup rápido em 48h para casos simples)

### Processo de Suporte

**Níveis de Suporte:**
- **Básico (incluso):** Suporte via email e portal
- **Premium (adicional):** Suporte prioritário em até 8h
- **Dedicado (enterprise):** Suporte prioritário em até 2h

**Canais:**
- Email
- WhatsApp
- Portal de suporte
- SLA conforme plano contratado

### Processo de Integrações

**Tipos de Integrações:**
- Conectores prontos para sistemas populares
- Desenvolvimento de integrações customizadas quando necessário
- Documentação e suporte técnico

### Processo de Escalabilidade

**Arquitetura Modular:**
- Permite escalar por módulos
- Infraestrutura cloud (AWS) escala automaticamente
- Clientes podem começar pequeno e expandir conforme crescem

### Processo de Cálculo Dinâmico de Planos

**Fluxo Identificado:**
```
Evolution API (recebe dados do cliente)
    ↓
JHIPSTER (sistema de cálculo)
    ↓
Cálculo de plano personalizado
    ↓
Retorna valores do plano
```

**Análise:**
- **Personalização:** Plano calculado dinamicamente
- **Automação:** Cálculo automático baseado em necessidades
- **Transparência:** Cliente vê exatamente o que está pagando

---

*Documento consolidado sobre fluxos, processos e arquitetura técnica*
*Última atualização: Dezembro 2025*
