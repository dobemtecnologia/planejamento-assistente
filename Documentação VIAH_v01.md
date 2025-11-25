# **VIAH – Vendas Inteligentes Automatizadas e Humanizadas**

**Framework Modular para Atendimento e Gestão Comercial**

## **1\. Introdução**

O **VIAH** é um framework modular que integra sistemas de atendimento, automação e gestão comercial, oferecendo uma solução robusta em um ecossistema unificado e escalável. Seus módulos trabalham juntos para suportar automações baseadas em fluxos pré-definidos e integrar diversas ferramentas de mercado, garantindo maior controle operacional, além de proporcionar uma experiência humanizada ao cliente com o uso das melhores inteligências artificiais disponíveis.

### **Principais módulos:**

* **VIAH Assistent AIVAH** – Assistente Inteligente de Vendas Automatizado para Humanos.

* **VIAH ERP** – Sistemas administrativos e financeiros

* **VIAH Omni** – Central de Gerenciamento Omnichannel de Atendimento

* **VIAH Connect** – Módulo de integração que conecta canais externos, como WhatsApp, e sistemas externos ao ecossistema **VIAH**

* **VIAH Conductor** – Orquestrador de automações inteligentes utilizando n8n.

* **VIAH Code** – Serviços de desenvolvimento personalizados para criar regras de negócio específicas para cada negócio via APIs, banco de dados e webapp, entre outros.

## 

## **2\. Arquitetura**

O **VIAH** é estruturado em módulos independentes que se comunicam por meio de APIs e conectores inteligentes, formando um ecossistema flexível, escalável e altamente integrável. Essa arquitetura permite personalização por cliente, automação de processos e gestão unificada de atendimento e operações comerciais.

### **2.1 | Visão Geral do Fluxo**

O funcionamento do **VIAH** é baseado em uma sequência inteligente de eventos que conecta clientes, automações, atendimento humano e sistemas de gestão:

* **Entrada do cliente:** Interações iniciadas via WhatsApp ou site são recebidas pelo **VIAH Link** (antigo Evolution API).

* **Condução conversacional:** O **VIAH Chat** (antigo Typebot) guia o cliente por fluxos automatizados.

* **Respostas inteligentes:** Quando necessário, o **VIAH AIVAH** assume o diálogo com IA avançada.

* **Automação de tarefas:** O **VIAH Conductor** (n8n) executa ações como agendamentos ou notificações.

* **Atendimento humano (opcional):** A conversa pode ser transferida para o **VIAH Omni** (Chatwoot).

* **Registro e gestão:** Todas as informações são integradas ao **VIAH ERP** (Odoo), garantindo controle operacional.

### **2.2 | Benefícios da Arquitetura Modular**

* Flexibilidade para adaptar regras e processos por cliente.

* Integração com ferramentas modernas via APIs abertas.

* Capacidade de automação total ou parcial de atendimentos.

* Centralização de dados em um núcleo de gestão confiável.

* Substituição ou evolução de módulos sem comprometer o ecossistema.

### **2.3 | Arquitetura em Camadas**

A estrutura técnica do VIAH pode ser organizada em quatro camadas funcionais:

1. **Camada de Entrada (Front-End de Comunicação)**

   * WhatsApp, Webchat (**VIAH Chat**)  
     Pontos de contato onde o cliente inicia a interação com a empresa.

2. **Camada de Inteligência**

   * **VIAH Chat**  
     Interface guiada que conduz fluxos automatizados.

   * **VIAH AIVAH**  
     Assistente de IA para atendimento natural e vendas automatizadas.

3. **Camada de Automações**

   * **VIAH Conductor (n8n)**  
     Executa lógicas de negócio, orquestra integrações e automatiza tarefas.

   * **VIAH Connect**   
     Atua como ponte entre canais externos e os módulos internos do VIAH.

4. **Camada de Backend e Gestão**

   * **VIAH Omni (Chatwoot)**  
     Atendentes humanos assumem o controle quando necessário.

   * **VIAH ERP (Odoo)**  
     Registra dados, gerencia operações comerciais, administrativas e financeiras.

## **3\. Módulos**

### **3.1 AIVAH –  Assistente Inteligente de Vendas Automatizado para Humanos**

O **AIVAH** é o assistente conversacional com inteligência artificial da solução **VIAH**. Projetado para operar de forma autônoma ou guiada, ele atua em duas modalidades complementares — otimizando processos de atendimento, vendas e suporte com alta adaptabilidade.

Capaz de compreender contextos complexos, aplicar regras de negócio personalizadas e integrar-se a múltiplos sistemas, o **AIVAH** é um agente estratégico no relacionamento com o cliente, promovendo uma experiência fluida e humanizada dentro do ecossistema **VIAH**.

#### **3.1.1 Atendimento Guiado**

Nessa modalidade, o **AIVAH** entrega uma experiência de atendimento estruturada e eficiente por meio de fluxos conversacionais pré-definidos, desenvolvidos com base em jornadas específicas de atendimento e vendas. Ele conduz o cliente de forma organizada e funcional, seguindo regras inteligentes alinhadas aos processos da empresa.

Interligado ao **VIAH Conductor** (n8n), **VIAH Connect** (Evolution API), **VIAH ERP** (ou ao ERP já utilizado pela empresa) e com suporte complementar do **VIAH Omni** (Central Omnichannel), esse fluxo permite:

* Triagem automatizada com base em regras e critérios definidos.

* Coleta precisa e guiada de dados como cadastros, preferências e formulários.

* Consultas inteligentes, como disponibilidade de estoque, status de pedidos e agendamentos.

* Agendamentos automatizados com controle de horários e limite de capacidade por faixa.

* Integração com o **VIAH ERP** para registrar ou consultar dados em tempo real — ou com sistemas próprios do cliente, conforme necessidade.

Quando necessário, o VIAH Omni pode **encaminhar a conversa para um atendente humano**, garantindo transição fluida, supervisão e continuidade do atendimento.

Mais do que um assistente, o **AIVAH** atua como recepcionista digital, agendador, consultor e braço comercial da operação, podendo ser treinado com dados específicos da empresa para atender diferentes **segmentos e contextos de negócio.**

### **3.1.2 Atendimento com Inteligência Artificial (IA)**

O **AIVAH** é capaz de oferecer atendimento autônomo, utilizando IA avançada para:

Nessa modalidade, o AIVAH atua com **inteligência contextual ativa**, utilizando modelos avançados de IA para oferecer interações naturais, inteligentes e conectadas aos processos da empresa.  
Ele compreende linguagem aberta, interpreta intenções complexas e responde de forma personalizada, sempre considerando o contexto da conversa, o histórico do cliente e os dados operacionais.

Entre suas capacidades neste modo estão:

* **Entender e interpretar consultas abertas e variadas**, mesmo fora dos fluxos pré-definidos.

* **Gerar respostas contextuais e personalizadas** com base em dados operacionais, preferências e histórico do cliente.

* **Executar decisões e acionar automações** conforme regras de negócio definidas no ecossistema **VIAH**.

* **Encaminhar o atendimento para um agente humano** via VIAH Omni quando identificar a necessidade de intervenção pessoal.

* **Redirecionar para o atendimento guiado**, caso reconheça que o cliente se beneficia mais de uma jornada estruturada.

Essa abordagem proporciona uma experiência conversacional mais fluida, responsiva e inteligente — elevando a qualidade do atendimento sem abrir mão do controle estratégico da operação.

 