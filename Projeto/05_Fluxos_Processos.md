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

## 📊 ANÁLISE ESTRATÉGICA DOS FLUXOGRAMAS MIRO

> **Fonte:** Análise profunda de 41 prints do quadro Miro  
> **Data de análise:** 2025  
> **Objetivo:** Compreender o modelo de negócio, fluxos operacionais e estratégias da Dobem Tecnologia

---

## 🎯 MODELO DE NEGÓCIO IDENTIFICADO: VERTICAL AI

### Definição Estratégica

A Dobem Tecnologia adota um **modelo de negócio Vertical AI**, que representa uma mudança fundamental de paradigma:

**Não é SaaS tradicional:**
- ❌ Não vende software como serviço genérico
- ✅ Vende **fluxos de otimização de operação** especializados

**Diferencial:**
- Especialização em nichos específicos de mercado
- Uso de Inteligência Artificial para automatizar processos únicos de cada setor
- Adaptação a qualquer negócio, mas com profundidade vertical

### Aplicação Prática: Caso Bira Veículos

**O Problema:**
No fluxo de operação de uma concessionária, existem várias tarefas repetitivas que são feitas por humanos porque não existe software capaz de atender aquela demanda específica.

**A Solução:**
Uma IA pode ser treinada para executar essas atividades, dividindo em pequenos agentes especializados que se integram para atender totalmente a demanda.

**Exemplo Concreto:**
- Extração de dados de uma carteira de habilitação
- Salvar no banco de dados
- Utilizar para formalizar contrato
- Utilizar para financiamento
- Utilizar para transferência do veículo

**Requisito Fundamental:**
Criar um fluxo de operação bem definido, onde a tarefa passa a ser previsível → logo mais possível de ser desenvolvida por uma IA.

### Estratégia de Venda

**Abordagem:**
- Criar várias soluções integradas utilizando IA
- Esse conjunto forma uma solução em um nicho específico de mercado
- As possibilidades são infinitas

**Valor Proposto:**
"Fluxos de otimização de operação" ao invés de "software"

---

## 💡 CONCLUSÕES SOBRE O MODELO DE NEGÓCIO

### Diferenciação Estratégica

**1. Vertical AI vs. SaaS Horizontal:**
- **Concorrentes tradicionais:** Oferecem soluções genéricas (chatbot, CRM, ERP)
- **Dobem:** Oferece **fluxos de otimização** especializados por setor
- **Vantagem:** Profundidade > Amplitude

**2. Personalização Profunda:**
- Não é "configuração" de software
- É **criação de agentes especializados** para processos únicos do cliente
- Cada cliente recebe uma solução adaptada ao seu negócio

**3. Ecossistema vs. Produto:**
- Não vende produtos isolados
- Vende **ecossistemas integrados** (ERP + Assistente + Automação + Atendimento)
- Valor agregado muito maior

### Proposta de Valor Única

**Para o Cliente:**
- "Não vendemos software, vendemos otimização de operação"
- "Automatizamos processos que só humanos faziam"
- "Criamos agentes especializados para seu negócio"

**Diferencial:**
- Entendimento profundo do negócio do cliente
- Mapeamento completo de processos
- Automação de tarefas que pareciam impossíveis de automatizar

### Análise de Preços e Estrutura Comercial

**Kits de Produtos:**
- **KIT SETUP STARTUP:** R$ 3.000,00
- **KIT VENDA ATENDIMENTO:** R$ 3.000,00
- **KIT SETUP PET:** R$ 3.000,00

**Estrutura de Preços Modular:**
- Componentes individuais com preços variáveis
- Licenças Odoo: Custo variável
- Número de workflows: Custo variável
- Número de assistentes IA: Custo variável
- APIs de IA: Custo variável (OpenAI, etc.)

**Análise:**
- **Modelo híbrido:** Setup inicial (kit) + custos variáveis (uso)
- **Escalabilidade:** Cliente paga pelo que usa
- **Flexibilidade:** Pode começar pequeno e escalar

---

## 🎯 DORES DO CLIENTE MAPEADAS

### Problemas Operacionais Identificados

**1. Falta de Visibilidade:**
- Empresas não sabem como vendedores se relacionam com clientes
- Não sabem se vendedores passam valores da empresa
- Não sabem se vendedor está atendendo bem

**2. Falta de Histórico:**
- Histórico de negociações fica com o vendedor
- Perda de informações importantes
- Dificuldade em resgatar oportunidades perdidas

**3. Falta de Gestão:**
- Sem gestão de atendimento centralizada
- Sem CRM para gerenciar oportunidades
- Sem gestão de funil automatizada

**4. Falta de Métricas:**
- Não sabe quais campanhas convertem mais
- Decisões sem base de dados
- Sem controle automático de leads

### Oportunidade de Mercado

**Conclusão:**
As empresas não precisam apenas de "um chatbot" ou "um CRM". Elas precisam de:
- **Visibilidade** sobre o que acontece no atendimento
- **Histórico** de todas as interações
- **Automação** de processos repetitivos
- **Métricas** para tomar decisões
- **Controle** sobre leads e oportunidades

**A Dobem resolve isso com um ecossistema integrado.**

---

## 💰 ANÁLISE DE VALOR ENTREGUE

### Valor para o Cliente

**Operacional:**
- Automação de processos repetitivos
- Redução de tempo de resposta
- Disponibilidade 24/7
- Escalabilidade sem contratar mais pessoas

**Estratégico:**
- Visibilidade sobre atendimento
- Histórico completo de interações
- Métricas para decisões
- Controle sobre leads e oportunidades

**Financeiro:**
- Redução de custos operacionais
- Aumento de conversão
- Melhor gestão de leads
- ROI mensurável

### Diferenciação vs. Concorrentes

**Concorrentes Tradicionais:**
- Chatbots genéricos
- CRMs isolados
- ERPs desconectados
- Soluções pontuais

**Dobem Tecnologia:**
- Ecossistema integrado
- Automação end-to-end
- Especialização por setor
- Fluxos de otimização de operação

---

## 🚀 PRÓXIMOS PASSOS ESTRATÉGICOS

### Desenvolvimento de Produto

**Prioridades:**
1. Finalizar MVP do EVAH
2. Criar mais kits por setor (além dos 3 atuais)
3. Desenvolver biblioteca de agentes reutilizáveis
4. Melhorar documentação de processos

### Go-to-Market

**Estratégias:**
1. Focar em setores específicos inicialmente
2. Criar cases de sucesso (Bira Veículos como primeiro)
3. Desenvolver materiais de venda por setor
4. Parcerias estratégicas

### Operações

**Melhorias:**
1. Padronizar processo de mapeamento de processos
2. Criar templates de implementação
3. Desenvolver ferramentas de cálculo de ROI
4. Sistema de métricas e acompanhamento

---

## 📝 OBSERVAÇÕES FINAIS

### Forças do Modelo

1. **Diferenciação clara:** Vertical AI é único no mercado
2. **Valor mensurável:** ROI tangível para clientes
3. **Escalabilidade técnica:** Arquitetura moderna e flexível
4. **Flexibilidade comercial:** Múltiplos modelos de preço

### Desafios

1. **Educação de mercado:** Cliente precisa entender o conceito de Vertical AI
2. **Complexidade de venda:** Requer entendimento profundo do negócio do cliente
3. **Tempo de implementação:** Mapear processos leva tempo
4. **Dependência de expertise:** Requer equipe técnica especializada

### Oportunidades

1. **Mercado em crescimento:** IA e automação em alta
2. **Dores reais:** Clientes têm problemas que a Dobem resolve
3. **Diferenciação:** Poucos concorrentes com modelo similar
4. **Escalabilidade:** Uma vez mapeado, pode replicar por setor

---

*Documento consolidado sobre fluxos, processos e arquitetura técnica*
*Última atualização: Dezembro 2025*
