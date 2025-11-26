# 📦 EVAH - Informações sobre o Produto

> **Documento consolidado sobre a plataforma EVAH e Evah Assistant**
> Informações sobre: plataforma, assistente virtual, agentes, funcionalidades, módulos e documentação técnica.

---

## 9. Documentação EVAH

### Arquivo: Documentação EVAH_v01.md# **EVAH – Vendas Inteligentes Automatizadas e Humanizadas**

# **EVAH – Vendas Inteligentes Automatizadas e Humanizadas**

**Framework Modular para Atendimento e Gestão Comercial**

## **1\. Introdução**

### **Principais módulos:**

* **EVAH Assistent Evah Assistant** – Assistente Inteligente de Vendas Automatizado para Humanos.

* **EVAH ERP** – Sistemas administrativos e financeiros

* **EVAH Omni** – Central de Gerenciamento Omnichannel de Atendimento

* **EVAH Connect** – Módulo de integração que conecta canais externos, como WhatsApp, e sistemas externos ao ecossistema **EVAH**

* **EVAH Conductor** – Orquestrador de automações inteligentes utilizando n8n.

* **EVAH Code** – Serviços de desenvolvimento personalizados para criar regras de negócio específicas para cada negócio via APIs, banco de dados e webapp, entre outros.

## 

## **2\. Arquitetura**

O **EVAH** é estruturado em módulos independentes que se comunicam por meio de APIs e conectores inteligentes, formando um ecossistema flexível, escalável e altamente integrável. Essa arquitetura permite personalização por cliente, automação de processos e gestão unificada de atendimento e operações comerciais.

### **2.1 | Visão Geral do Fluxo**

O funcionamento do **EVAH** é baseado em uma sequência inteligente de eventos que conecta clientes, automações, atendimento humano e sistemas de gestão:

* **Entrada do cliente:** Interações iniciadas via WhatsApp ou site são recebidas pelo **EVAH Link** (antigo Evolution API).

* **Condução conversacional:** O **EVAH Chat** (antigo Typebot) guia o cliente por fluxos automatizados.

* **Respostas inteligentes:** Quando necessário, o **EVAH Evah Assistant** assume o diálogo com IA avançada.

* **Automação de tarefas:** O **EVAH Conductor** (n8n) executa ações como agendamentos ou notificações.

* **Atendimento humano (opcional):** A conversa pode ser transferida para o **EVAH Omni** (Chatwoot).

* **Registro e gestão:** Todas as informações são integradas ao **EVAH ERP** (Odoo), garantindo controle operacional.

### **2.2 | Benefícios da Arquitetura Modular**

* Flexibilidade para adaptar regras e processos por cliente.

* Integração com ferramentas modernas via APIs abertas.

* Capacidade de automação total ou parcial de atendimentos.

* Centralização de dados em um núcleo de gestão confiável.

* Substituição ou evolução de módulos sem comprometer o ecossistema.

### **2.3 | Arquitetura em Camadas**

A estrutura técnica do EVAH pode ser organizada em quatro camadas funcionais:

1. **Camada de Entrada (Front-End de Comunicação)**

   * WhatsApp, Webchat (**EVAH Chat**)  
     Pontos de contato onde o cliente inicia a interação com a empresa.

2. **Camada de Inteligência**

   * **EVAH Chat**  
     Interface guiada que conduz fluxos automatizados.

   * **EVAH Evah Assistant**  
     Assistente de IA para atendimento natural e vendas automatizadas.

3. **Camada de Automações**

   * **EVAH Conductor (n8n)**  
     Executa lógicas de negócio, orquestra integrações e automatiza tarefas.

   * **EVAH Connect**   
     Atua como ponte entre canais externos e os módulos internos do EVAH.

4. **Camada de Backend e Gestão**

   * **EVAH Omni (Chatwoot)**  
     Atendentes humanos assumem o controle quando necessário.

   * **EVAH ERP (Odoo)**  
     Registra dados, gerencia operações comerciais, administrativas e financeiras.

## **3\. Módulos**

### **3.1 Evah Assistant –  Assistente Inteligente de Vendas Automatizado para Humanos**

O **Evah Assistant** é o assistente conversacional com inteligência artificial da solução **EVAH**. Projetado para operar de forma autônoma ou guiada, ele atua em duas modalidades complementares — otimizando processos de atendimento, vendas e suporte com alta adaptabilidade.

Capaz de compreender contextos complexos, aplicar regras de negócio personalizadas e integrar-se a múltiplos sistemas, o **Evah Assistant** é um agente estratégico no relacionamento com o cliente, promovendo uma experiência fluida e humanizada dentro do ecossistema **EVAH**.

#### **3.1.1 Atendimento Guiado**

Nessa modalidade, o **Evah Assistant** entrega uma experiência de atendimento estruturada e eficiente por meio de fluxos conversacionais pré-definidos, desenvolvidos com base em jornadas específicas de atendimento e vendas. Ele conduz o cliente de forma organizada e funcional, seguindo regras inteligentes alinhadas aos processos da empresa.

Interligado ao **EVAH Conductor** (n8n), **EVAH Connect** (Evolution API), **EVAH ERP** (ou ao ERP já utilizado pela empresa) e com suporte complementar do **EVAH Omni** (Central Omnichannel), esse fluxo permite:

* Triagem automatizada com base em regras e critérios definidos.

* Coleta precisa e guiada de dados como cadastros, preferências e formulários.

* Consultas inteligentes, como disponibilidade de estoque, status de pedidos e agendamentos.

* Agendamentos automatizados com controle de horários e limite de capacidade por faixa.

* Integração com o **EVAH ERP** para registrar ou consultar dados em tempo real — ou com sistemas próprios do cliente, conforme necessidade.

Quando necessário, o EVAH Omni pode **encaminhar a conversa para um atendente humano**, garantindo transição fluida, supervisão e continuidade do atendimento.

Mais do que um assistente, o **Evah Assistant** atua como recepcionista digital, agendador, consultor e braço comercial da operação, podendo ser treinado com dados específicos da empresa para atender diferentes **segmentos e contextos de negócio.**

### **3.1.2 Atendimento com Inteligência Artificial (IA)**

O **Evah Assistant** é capaz de oferecer atendimento autônomo, utilizando IA avançada para:

Nessa modalidade, o Evah Assistant atua com **inteligência contextual ativa**, utilizando modelos avançados de IA para oferecer interações naturais, inteligentes e conectadas aos processos da empresa.  
Ele compreende linguagem aberta, interpreta intenções complexas e responde de forma personalizada, sempre considerando o contexto da conversa, o histórico do cliente e os dados operacionais.

Entre suas capacidades neste modo estão:

* **Entender e interpretar consultas abertas e variadas**, mesmo fora dos fluxos pré-definidos.

* **Gerar respostas contextuais e personalizadas** com base em dados operacionais, preferências e histórico do cliente.

* **Executar decisões e acionar automações** conforme regras de negócio definidas no ecossistema **EVAH**.

* **Encaminhar o atendimento para um agente humano** via EVAH Omni quando identificar a necessidade de intervenção pessoal.

* **Redirecionar para o atendimento guiado**, caso reconheça que o cliente se beneficia mais de uma jornada estruturada.

Essa abordagem proporciona uma experiência conversacional mais fluida, responsiva e inteligente — elevando a qualidade do atendimento sem abrir mão do controle estratégico da operação.

### Arquivo: EVAH – Vendas Inteligentes Automatizadas e Humanizadas.md# EVAH – Vendas Inteligentes Automatizadas e Humanizadas

## Framework Modular para Atendimento e Gestão Comercial

## *Framework \=  Quadro de ferramentas, funcionalidades genéricas para serem implementadas em um negócio específico.*

## 1\. Introdução

#### **Principais módulos:**

    • **EVAH Assistent Evah Assistant** – Assistente Inteligente de Vendas Automatizado para Humanos.  
    • **EVAH ERP** – Sistemas administrativos e financeiros  
    • **EVAH Omni** – Central de Gerenciamento Omnichannel de Atendimento  
    • **EVAH Connect** – Módulo de integração que conecta canais externos, como WhatsApp, e sistemas externos ao ecossistema **EVAH**  
    • **EVAH Maestro** – Orquestrador de automações inteligentes utilizando n8n (a ferramenta que automatiza o processo).  
    • **EVAH Code** – Serviços de desenvolvimento personalizados para criar regras de negócio específicas para cada negócio via APIs, banco de dados e webapp, entre outros.

## **2\. Módulos**

### **2.1 EVAH Assistent Evah Assistant Assistente Inteligente de Vendas Automatizado para Humanos.**

O **Evah Assistant** é o assistente conversacional com inteligência artificial da solução **EVAH**. Projetado para operar de forma inteligente e supervisionada, ele atua em duas modalidades complementares — otimizando processos de atendimento, vendas e suporte com alta adaptabilidade.  
Capaz de compreender contextos complexos, aplicar regras de negócio personalizadas e integrar-se a múltiplos sistemas, o **Evah Assistant** é um agente estratégico no relacionamento com o cliente, promovendo uma experiência fluida e humanizada dentro do ecossistema **EVAH**.

#### Funcionalidades Principais:

* Recepcionista digital  
* Assistente comercial  
* Agente de suporte técnico  
* Triagem Inteligente de Demandas  
  Interpreta a solicitação do cliente em linguagem natural, aplica regras de negócio, prioridades e perfis de atendimento para direcionamento automatizado da jornada.

* Condução por Jornadas Estruturadas  
  Leva o cliente por fluxos pré-definidos, com lógica condicional, pontos de validação e ramificações conforme suas escolhas e comportamentos.

* Compreensão de Linguagem Aberta  
  Entende mensagens livres, reconhece múltiplas intenções, mantém o contexto e se adapta dinamicamente às mudanças na conversa.

* Respostas Inteligentes e Contextuais  
  Gera respostas com base no histórico do cliente, dados em tempo real e tom ajustado ao canal e perfil de atendimento.

* Coleta Guiada e Estruturada de Dados  
  Realiza coleta de informações por meio de formulários interativos, com validações automáticas e enriquecimento de dados.

* Consultas em Tempo Real  
  Acessa sistemas externos via API para responder sobre status de pedidos, estoques, condições comerciais, produtos, localização e mais.

* Agendamento Automatizado de Serviços  
  Gerencia agendas com base em disponibilidade, capacidade máxima por horário, tipo de serviço, regras específicas e perfis do cliente.

* Execução de Ações Baseadas em Regras de Negócio  
  Dispara automaticamente ações como:  
  * Criação de registros no ERP ou CRM  
  * Atualização de status  
  * Envio de e-mails ou mensagens  
  * Encaminhamentos e notificações internas

* Encaminhamento Inteligente para Agentes Humanos  
  Realiza a transição para atendimento humano mantendo o histórico, o contexto e os dados coletados, seja via EVAH Omni ou plataforma integrada.

* Redirecionamento Estratégico de Jornada  
  Identifica quando há necessidade de suporte avançado ou mudança de rota, redirecionando o cliente para um fluxo mais adequado.

* Integração com ERP ou Sistema de Gestão  
  Permite consultar, criar ou atualizar dados operacionais diretamente nos sistemas da empresa (estoque, financeiro, pré-vendas, ordens de serviço, etc.).

* Aprendizado e Otimização Contínua  
  Monitora padrões de uso, identifica gargalos e ajusta comportamentos e fluxos automaticamente para otimizar a experiência.

* Conversão Interativa de Áudio e Texto  
  Permite entrada e saída por voz, com transcrição automática de áudio para texto e resposta em formato multimodal.

* Análise de Imagens  
  Interpreta imagens enviadas pelo cliente, podendo transcrever conteúdo ou identificar elementos visuais conforme o contexto da interação.  

* Roteamento de Conversa Baseado em Perfil de Cliente  
  Personaliza jornadas de atendimento conforme histórico, comportamento ou classificação do cliente.  
  Ex: clientes VIP seguem fluxos mais rápidos ou recebem ofertas exclusivas.

* Respostas Contextuais Dinâmicas com Tom Adaptativo  
  Ajusta automaticamente o tom de comunicação (formal, técnico ou amigável) com base no canal e no perfil do cliente.

* Orquestração Multi-Função (Comercial, Suporte e Pós-venda)  
  Um único Evah Assistant pode desempenhar múltiplos papéis de forma modular, alternando comportamentos conforme horário, contexto ou setor da empresa.

* Agendamento Inteligente com Lógica Avançada de Capacidade  
  Aplica regras dinâmicas para priorização de agendas conforme urgência, SLA, campanha ativa ou tipo de serviço.  
  Ex: em datas sazonais como Black Friday, prioriza agendamentos com foco comercial.

* Interação Multimodal (Texto, Áudio e Imagem)  
  Permite ao cliente interagir via texto, áudio ou imagem, com interpretação e extração automática de dados a partir dos arquivos enviados.

* Motor de Regras Personalizado (Workflow Administrativo)  
  Possibilita a criação e manutenção de regras de negócio diretamente no painel administrativo, sem a necessidade de intervenção técnica.

* Gatilhos Inteligentes por Emoção ou Urgência  
  Detecta sinais de frustração, ansiedade ou urgência nas mensagens e executa ações como redirecionamento automático para atendimento humano.

* Recomendações Personalizadas com Base em Dados Internos  
  Sugere produtos, serviços ou soluções com base em histórico de navegação, compras anteriores ou perfil de uso do cliente.

* Integração Nativa com BI para Aprendizado Contínuo  
  Exporta métricas e eventos de atendimento para ferramentas de BI (como Power BI, Metabase, etc.), ajustando fluxos com base em indicadores-chave de performance (KPIs).

* Experiência Multi Empresa / Multimarcas com Personalidade Adaptável  
  Adapta tom de voz, vocabulário, identidade e comportamento conforme a marca ou unidade da empresa que o cliente estiver acessando.

### **2.2 EVAH Omni – Central de Gerenciamento Omnichannel de Atendimento (Chatwoot)**

O **EVAH** Omni é a central de gerenciamento omnichannel baseada na plataforma Chatwoot, integrada ao ecossistema **EVAH** para oferecer um atendimento unificado, eficiente e supervisionado. Ele possibilita que atendentes humanos assumam o controle das conversas iniciadas nos canais digitais, garantindo continuidade, qualidade e personalização no relacionamento com o cliente.

* **Canais de Atendimento Integrados**  
  * Suporte para WhatsApp, Facebook Messenger, Instagram, Twitter, e-mail, chat web e SMS  
  * Consolidação das conversas em uma interface única  
  * Atualização em tempo real das mensagens

* **Gestão de Conversas**  
  * Caixa de entrada unificada, com filtros por status, prioridade e etiquetas personalizadas  
    Histórico completo das interações, incluindo transferências, anexos e notas internas  
  * Atribuição manual e automática de conversas para agentes  
    Regras de escalonamento e transferência entre atendentes  
  * Controle de pausas, retomadas e encerramentos de atendimentos

* **Automação e Regras de Atendimento**  
  * Configuração de respostas rápidas e mensagens automáticas (boas-vindas, ausência)  
    Gatilhos baseados em palavras-chave, tempo de espera, canal e outras condições  
  * Modelos pré-definidos para padronização e agilidade no atendimento  
  * Notificações automáticas para agentes e clientes

* **Colaboração Interna e Supervisão**  
  * Comunicação interna entre agentes via notas privadas e comentários em conversas  
  * Monitoramento em tempo real por supervisores, com possibilidade de intervenção  
  * Gestão de usuários, permissões, equipes e filas de atendimento

* **Relatórios e Análises**  
  * Dashboards com KPIs como tempo médio de resposta, volume de atendimentos e satisfação do cliente  
  * Exportação de relatórios para análises externas  
    Histórico analítico para avaliação contínua da qualidade do atendimento

* **Integração e Extensibilidade**  
  * APIs abertas para integração com módulos EVAH, ERP e CRM  
  * Webhooks para captura de eventos e automações avançadas  
  * Suporte para plugins e extensões customizadas

### **2.3 EVAH Connect – Módulo de integração que conecta canais**

O **EVAH** Connect é o módulo responsável por integrar canais externos, como WhatsApp, e sistemas externos ao ecossistema **EVAH**, utilizando a Evolution API. Esta integração permite a comunicação fluida e sincronizada entre plataformas, centralizando o atendimento e otimizando processos.

#### Funcionalidades Principais

* **Integração com Canais Digitais**  
  * Oferece suporte completo para integração com o WhatsApp por meio da Evolution API. Essa integração utiliza uma biblioteca baseada em Baileys, que implementa uma interface programática para o WhatsApp Web  
  * Possibilidade de integração com outros canais, como Instagram e Messenger, conforme disponibilidade da Evolution API.

* **Sincronização de Mensagens e Contatos**  
  * Importação automática de mensagens e contatos do canal externo para o Chatwoot.  
  * Sincronização bidirecional, permitindo o envio e recebimento de mensagens entre o Chatwoot e os canais externos.

* **Gerenciamento de Conversas**  
  * Criação e gerenciamento de conversas no Chatwoot a partir das interações nos canais externos.  
  * Atribuição de conversas a agentes específicos, com possibilidade de reabertura de conversas pendentes.

* **Automação e Regras de Atendimento**  
  * Configuração de regras automáticas para distribuição de mensagens, respostas rápidas e mensagens de ausência.  
  * Gatilhos acionados por palavras-chave, tempo de espera ou outras condições configuráveis.

* **Segurança e Confiabilidade**  
  * Criptografia de dados e autenticação robusta nas integrações.  
  * Monitoramento de disponibilidade e falhas para garantia de continuidade.

* **Extensibilidade e Customização**  
  * Suporte para plugins e extensões, permitindo a personalização das funcionalidades conforme as necessidades do cliente.  
  * APIs abertas para integração com outros sistemas e ferramentas.

### **2.4 EVAH Maestro – Orquestrador de automações inteligentes utilizando n8n**

O **EVAH Conductor** é o núcleo de automações inteligentes do ecossistema **EVAH**, utilizando a plataforma open source **n8n** para criar, gerenciar e executar fluxos complexos que integram múltiplos sistemas, canais e processos empresariais. Seu design modular e escalável permite que a operação seja automatizada com alta flexibilidade, garantindo agilidade, controle e precisão.

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

* Suporte Omnichannel  
  Gerencia fluxos que envolvem diferentes canais simultaneamente, garantindo que a operação mantenha consistência e integração total.

### **2.5 EVAH Code – Serviços de desenvolvimento personalizados**

O módulo **EVAH Code** é responsável por atender demandas específicas que não se enquadram em soluções prontas do ecossistema **EVAH**. Atua como uma camada de extensão flexível, oferecendo serviços sob medida para personalização, automação avançada e integração de sistemas legados ou proprietários.

#### Funcionalidades principais

##### 🔹 Criação de Componentes Exclusivos

* Desenvolvimento de funcionalidades específicas para atender requisitos únicos do cliente, respeitando os padrões e diretrizes do EVAH.

##### 🔹 Integrações com Sistemas Legados ou Proprietários

* Conexão de ERPs, CRMs, bancos de dados, ou APIs internas com os módulos do EVAH, utilizando protocolos seguros e escaláveis.

##### 🔹 Extensão de Fluxos e Automações Complexas

* Implementação de rotinas ou processos que exigem lógica avançada, incluindo manipulação de dados, cálculos personalizados ou regras de negócio complexas.

##### 🔹 Personalização de Interface e Experiência Conversacional

* Ajustes visuais ou de comportamento dos assistentes e interfaces, adaptando a experiência conforme a identidade da empresa ou público-alvo.

##### 🔹 Criação de APIs Customizadas

* Desenvolvimento de APIs RESTful para facilitar a comunicação entre o EVAH e sistemas externos que não possuem conectores diretos.

##### **🔹** Suporte a Projetos Especiais e Provas de Conceito

* Execução de projetos exploratórios, integrações pontuais e protótipos sob demanda, com ciclos curtos de entrega e validação.

##### **🔹 Gerenciamento de Ciclo de Vida do Código**

* Controle de versões, testes automatizados e boas práticas de deploy, garantindo a estabilidade e evolução contínua das personalizações.

###  **2.6 EVAH ERP – Sistemas administrativos e financeiros**

O EVAH ERP é um módulo opcional de gestão administrativa, financeira e operacional. Totalmente integrado ao ecossistema EVAH, oferece funcionalidades robustas e modulares para empresas que não possuem ou desejam modernizar seu sistema atual.

**Importante:** Caso o cliente já possua um ERP próprio, não há qualquer impedimento. O **EVAH** integra-se a sistemas externos por meio de conectores nativos ou personalizados via Evolution API.

#### **Núcleos Funcionais**

##### **🔹 Gestão Financeira**

* Contas a pagar e a receber com controle por status, vencimento, centro de custo e integração bancária.  
* Conciliação bancária automatizada por importação de extratos.  
* Fluxo de caixa com projeções e relatórios de saldo.  
* Emissão de boletos, lembretes automáticos e integração com gateways de pagamento.  
* Rateios e classificações financeiras por centro de custo.

##### **🔹 Gestão Comercial**

* Cadastro completo de produtos e serviços com controle de estoque.  
* Geração de orçamentos e propostas com aprovação automática ou manual.  
* Gestão de pedidos de venda com rastreamento completo até a entrega.

##### **🔹 Compras e Estoque**

* Solicitações de compra com fluxo de aprovação.  
* Controle de estoque com alertas, inventário e rastreamento por lote.  
* Geração e acompanhamento de pedidos a fornecedores com comparativo de cotações.

##### **🔹 Pessoas (RH Operacional)**

* Cadastro e gestão de colaboradores com histórico e documentos.  
* Integração com folha externa e controle de repasses.  
* Gerenciamento de benefícios, comissões e reembolsos.

##### **🔹 Fiscal e Documental**

* Emissão de NF-e, NFC-e e boletos diretamente no sistema.  
* Cálculo e gestão de impostos com exportação para contador.  
* Armazenamento digital de documentos fiscais e contratuais.

##### **🔹 Integrações Nativas**

* Integração bancária (boletos, Pix, extratos).  
* Exportação contábil para sistemas externos.  
* Integração com marketplaces e ERPs externos via Evolution API.

##### **🔹 Relatórios Gerenciais**

* Dashboards em tempo real com KPIs financeiros e comerciais.  
* Exportação de dados em CSV, PDF, Excel ou API.  
* Notificações automáticas por e-mail ou sistema.  
---

### Arquivo: EVAH – Vendas Inteligentes Automatizadas e Humanizadas - Módulos EVAH.md# EVAH – Vendas Inteligentes Automatizadas e Humanizadas - Módulos EVAH

---

                                                                       Assistente Inteligente de Vendas Automatizado para Humanos. O Evah Assistant é o assistente conversacional com inteligência artificial da solução EVAH. Projetado para operar de forma inteligente e supervisionada, ele atua em duas modalidades complementares —
                                                                                                                                                           otimizando processos de atendimento, vendas e suporte com alta adaptabilidade.
                 EVAH Assistant: "Evah Assistant"                                  Capaz de compreender contextos complexos, aplicar regras de negócio personalizadas e integrar-se a múltiplos sistemas, o Evah Assistant é um agente estratégico no relacionamento com o cliente, promovendo uma experiência fluida e humanizada dentro do
                                                                                                                                                                                           ecossistema EVAH.

                                  Componente                                                                                          Descrição                                                                 Tipo cobrança         Qual custo                            Custos               Valor custo            Req Ref
A1.1    Hospedagem automática em links do Typebot                                                                                                                                                             Pacote
                                                                     -Funcionalidade do Typebot, uma plataforma de criação de chatbots conversacionais, onde o próprio Typebot hospeda o seu bot e gera um link                        TypeBot
                                                                                                                                                                                                                direto para ele funcionar                                  R$ 100,00
                                                                                                                                                                                                                                          na web – sem que você precise configurar                 R$domínio
                                                                                                                                                                                                                                                                                   um servidor ou um  100,00 próprio.      1
A1.2    Publicação como widget em sites (iframe ou script)           -No Typebot significa que você pode inserir o seu chatbot diretamente em qualquer site, de duas formas:                                    Pacote                TypeBot                              R$ 100,00               R$ 100,00               1
A1.3    AgenteIA - Agendamentos via Google Calendar                  - Sincroniza e gerencia eventos no Google Calendar via API oficial Google. Permite criação, consulta e notificações via fluxos do Evah Assistant.   Pacote                API Google ,Open IA                   R$ 0,02                 R$ 0,02               150
                                                                     - Permite que o Evah Assistant gerencie arquivos no Google Drive do cliente, com upload, download, organização e controle de permissões via API
A1.4    AgenteIA - Gestão de arquivos via Google Drive                                                                                                                                                          Pacote                API Google ,Open IA                   R$ 0,02                 R$ 0,02
                                                                     oficial Google Drive.                                                                                                                                                                                                                                25
                                                                     - Permite ao Evah Assistant extrair dados de páginas web em tempo real para alimentar fluxos com informações externas, como preços, prazos,
A1.5    AgenteIA - Consultas Web (Web Scraping)                                                                                                                                                                 Pacote                API Webscraping, Open IA              R$ 0,00                 R$ 0,00
                                                                     status ou disponibilidade de serviços.                                                                                                                                                                                                               25
A1.6    AgenteIA - Gestão Lead no CRM                                - Habilita o Evah Assistant a registrar novos leads diretamente no CRM do cliente com base em interações, formulários ou gatilhos específicos.      Pacote                Open IA                               R$ 0,02                 R$ 0,02               180
                                                                     - Capacita o Evah Assistant a receber mensagens de voz enviadas pelos usuários em canais compatíveis, armazenando e processando o
A1.7    AgenteIA - Recebimento de mensagens em áudio                                                                                                                                                            Pacote                Open IA                               R$ 0,02                 R$ 0,02
                                                                     conteúdo.                                                                                                                                                                                                                                            250
                                                                     - Permite que o Evah Assistant analise imagens enviadas por usuários, reconhecendo elementos visuais, textos ou padrões relevantes para o
A1.8    AgenteIA - Capacidade de identificar o conteudo de imagens                                                                                                                                              Pacote                Open IA                               R$ 0,02                 R$ 0,02
                                                                     atendimento.                                                                                                                                                                                                                                         80
        AgenteIA - Redirecionamento para atendente humano            - Garante que o Evah Assistant identifique contextos em que a interação requer intervenção humana e transfira o atendimento para um operador da
A1.9                                                                                                                                                                                                            Pacote                Open IA                               R$ 0,02                 R$ 0,02
        quando necessário                                            equipe em tempo real.                                                                                                                                                                                                                                50
A1.10   AgenteIA - Capacidade de identificar a inteção do usuario    - Comforme a conversa do interlocutor cliente, o AgenteIA indentifica qual a inteção do cliente                                            Pacote                Open IA                               R$ 0,02                 R$ 0,02               70
                                                                     - Permite que o Evah Assistant consulte em tempo real a disponibilidade de produtos no ERP do cliente, exibindo quantidade, localização e status
A1.11   AgenteIA - Gestão produtos no estoque do ERP                                                                                                                                                            Pacote                Open IA                               R$ 0,02                 R$ 0,02
                                                                     do estoque.                                                                                                                                                                                                                                          200
        AgenteIA - Consulta detalhes de um produto selecionado       - Habilita o Evah Assistant a retornar informações específicas de um produto com base na seleção do usuário, como descrição, especificações
A1.12                                                                                                                                                                                                           Pacote                Open IA                               R$ 0,02                 R$ 0,02
        pelo usuário                                                 técnicas, preços e variantes.                                                                                                                                                                                                                        150
A1.13   AgenteIA - Exibe fotos de um produto                         - Capacita o Evah Assistant a apresentar imagens associadas ao produto consultado, melhorando a experiência visual do atendimento                   Pacote                Open IA                               R$ 0,02                 R$ 0,02               200
                                                                     - Permite ao Evah Assistant retornar valores atualizados de veículos conforme a Tabela FIPE, útil para negociações, simulações e cotações
A1.14   AgenteIA - Consulta tabela FIPE do veiculo                                                                                                                                                              Pacote                Open IA, API FiPE                     R$ 0,02                 R$ 0,02
                                                                     automotivas                                                                                                                                                                                                                                          100
A1.15   AgenteIA - Wiki de Empresa                                   - Detetm todas as informações da empresa                                                                                                   Pacote                Open IA                               R$ 0,02                 R$ 0,02               100
                                                                     - Permite simular condições de pagamento em tempo real, oferecendo ao cliente transparência e agilidade na negociação. Integrado ao
                                                                     atendimento, ele calcula parcelas, juros e prazos de forma personalizada, considerando as regras da instituição financeira.
                                                                     - Simulação imediata de parcelas e prazos
A1.16   AgenteIA - Calculo de Financiamento                                                                                                                                                                     Pacote                Open IA                               R$ 0,02                 R$ 0,02
                                                                     - Integração com taxas e condições de parceiros financeiros
                                                                     - Apresentação clara e personalizada durante o atendimento
                                                                     - Apoio à decisão de compra do cliente, sem precisar sair da conversa                                                                                                                                                                                100
                                                                     - Ele permite processar transações dentro do fluxo de atendimento, seja em vendas online ou presenciais, garantindo integração com
                                                                     múltiplos provedores.
                                                                     - Suporte a diferentes métodos de pagamento (cartão, Pix, boleto, etc.)
A1.17   AgenteIA - Gateway de Pagamento                                                                                                                                                                         Demanda               Exemplo: Pagseguro                    R$ 3,50                 R$ 3,50
                                                                     - Integração transparente com o CRM e ERP
                                                                     - Confirmações em tempo real dentro do atendimento
                                                                     - Segurança e conformidade com padrões de mercado                                                                                                                                                                                                     0
        AgenteIA - Direcionar para atendentes por ordem              - Deve ser definido uma lista de vendedores ordenada por um periodo pré-definido (em dias) onde o ciclo se repete quando chega no ultimo
A1.18                                                                                                                                                                                                         Adesao                  Open IA                               R$ 0,02                 R$ 0,02
        programada                                                   . Deve ser rotacionado também a ordem dos venderes para ter o maximo de oportunidades pra cada                                                                                                                                                       120
        AgenteIA - Comparador de preços para avaliar valor do bem
A1.19                                                                - Avaliação do bem a ser dado como pagamento, ou parte do pagamento no valor total de compra do bem a ser comprado.                        Pacote                Open IA                               R$ 0,02                 R$ 0,02
        de entrada carro/moto/imóvel de entrada                                                                                                                                                                                                                                                                           50
                                                                     - Garante que o Evah Assistant entenda e memorize informações fornecidas durante a conversa, mantendo coerência entre interações e
A1.20   AgenteIA - Capacidade de manter contexto de conversação                                                                                                                                                 Pacote                Open IA, Zep                          R$ 0,07                 R$ 0,07
                                                                     personalizando o atendimento.                                                                                                                                                                                                                        150
                                                                     - Conecta o Evah Assistant à API oficial do WhatsApp (Meta), mantendo os mesmos recursos de mensagens e mídias, mas com vantagens
        Atendimento via canal Whatsapp (Meta - API Oficial
A1.22                                                                adicionais: conformidade total com as políticas do WhatsApp, acesso a recursos exclusivos liberados primeiro na API oficial e suporte direto Adesao              API Meta                              R$ 0,03                 R$ 0,03
        WhatsApp)
                                                                     via provedores autorizados. Ideal para operações que exigem alto nível de governança e relacionamento corporativo com a Meta.
A1.23   Atendimento via canal Whatsapp Evolution API                                                                                                                                                         Pacote
                                                                     Evolution API é uma API de atendimento via WhatsApp, fornecida por empresas como 360dialog, Z-API, Cloud API, entre outras. Ela permite que ferramentas externasEvolution API chatbots, e plataformas
                                                                                                                                                                                                                                      (como CRMs,                        R$como
                                                                                                                                                                                                                                                                            100,00              R$ 100,00
                                                                                                                                                                                                                                                                                o Typebot) se conectem ao WhatsApp de forma
                                                                                                                                                                                                                                                                                                                       1    automatizada e profissional
                                                                     - Capacita o Evah Assistant a atender diretamente via mensagens do Instagram, respondendo a DMs, interações com stories e gatilhos de
A1.24   Atendimento via canal Instagram                                                                                                                                                                         Adesao                API Meta                              R$ 0,03                 R$ 0,03
                                                                     publicações.                                                                                                                                                                                                                                        1000
                                                                     - Integra o Evah Assistant ao Messenger do Facebook via API oficial, permitindo envio e recebimento de mensagens, execução de fluxos
A1.25   Atendimento via canal Facebook Messenger                                                                                                                                                                Adesao                API Meta                              R$ 0,03                 R$ 0,03
                                                                     automatizados e encaminhamento para atendente humano.                                                                                                                                                                                               1000
                                                                     - Integra o Evah Assistant ao Telegram via API oficial gratuita, permitindo envio e recebimento de mensagens, execução de fluxos automatizados e
A1.26   Atendimento via canal Telegram                                                                                                                                                                          Adesao                                                     R$ 100,00               R$ 100,00
                                                                     encaminhamento para atendente humano quando necessário.                                                                                                                                                                                               0
                                                                     - Integra o Evah Assistant a widgets de chat em sites (WebChat), permitindo conversas em tempo real com visitantes, execução de fluxos
A1.27   Atendimento via canal WebChat (chat do site)                                                                                                                                                            Adesao                Servidor Chatwoot                    R$ 82,20                R$ 82,20
                                                                     automatizados, coleta de dados e redirecionamento para atendentes humanos quando necessário.                                                                                                                                                          0
A1.28   Assistentes de IA                                            É um assistente para uma determinada demanda, exe: Asistente para SAC, Assitente para vendas, outro para...                                Pacote                                                                             R$ 500,00               1
A1.29   Agente IA - Assistente Corporativo                                                                                                                                                                      Adesao                Open IA, Zep                          R$ 0,02                 R$ 0,02              1000
                         EVAH ERP                                        O EVAH ERP é um módulo opcional de gestão administrativa, financeira e operacional. Totalmente integrado ao ecossistema EVAH, oferece funcionalidades robustas e modulares para empresas que não possuem ou desejam modernizar seu sistema atual.
B1.1    Site                                                         Criador de Sites Enterprise                                                                                                                                                                                                   R$ 250,00
B1.2    E-Commerce                                                   Venda seus produtos online                                                                                                                                                                                                    R$ 500,00
B1.3    Blog                                                                                                                                                                                                                                                                                       R$ 250,00
B1.4    Vendas                                                       De cotações a faturas                                                                                                                                                                                                          R$ 1,23
B1.5    Restaurante                                                  Extensões de restaurante para o ponto de venda                                                                                                                                                                                 R$ 1,23
B1.6    Faturamento                                                  Faturas, pagamentos, acompanhamentos e sincronização bancária                                                                                                                                                                  R$ 1,23
B1.7    CRM                                                          Rastreie leads e feche oportunidades                                                                                                                                                                                           R$ 1,23
B1.8    Fabricação II (Licença)                                      Ordens de trabalho, planejamento, relatórios de estoque.                                                                                                                                                                       R$ 1,23
                                                     Assistente Inteligente de Vendas Automatizado para Humanos. O Evah Assistant é o assistente conversacional com inteligência artificial da solução EVAH. Projetado para operar de forma inteligente e supervisionada, ele atua em duas modalidades complementares —
                                                                                                                                         otimizando processos de atendimento, vendas e suporte com alta adaptabilidade.
                   EVAH Assistant: "Evah Assistant"              Capaz de compreender contextos complexos, aplicar regras de negócio personalizadas e integrar-se a múltiplos sistemas, o Evah Assistant é um agente estratégico no relacionamento com o cliente, promovendo uma experiência fluida e humanizada dentro do
                                                                                                                                                                         ecossistema EVAH.

                                Componente                                                                              Descrição                                                          Tipo cobrança          Qual custo                            Custos               Valor custo            Req Ref
B1.9    Inventário                                 Gerencie suas atividades de estoque e logística                                                                                                                                                                              R$ 1,23
B1.10   Financeiro (Licença)                       Gerencie a contabilidade financeira e analítica                                                                                                                                                                              R$ 1,23
B1.11   Conhecimento                               Centralize, gerencie, compartilhe e amplie sua biblioteca de conhecimentos                                                                                                                                                   R$ 1,23
B1.12   Compras                                    Pedidos de compra, licitações e acordos                                                                                                                                                                                      R$ 1,23
B1.13   Ponto de Venda                             Interface de PDV fácil de usar para lojas e restaurantes                                                                                                                                                                     R$ 1,23
B1.14   Projetos                                   Organize e planeje seus projetos                                                                                                                                                                                             R$ 1,23
B1.15   Fabricação                                 Ordens de produção e LMs                                                                                                                                                                                                     R$ 1,23
B1.16   Marketing por E-mail                       Crie, envie e acompanhe e-mails                                                                                                                                                                                              R$ 1,23
B1.17   Planilhas de Horas (Licença)               Rastreie as horas dos funcionários em tarefas                                                                                                                                                                                R$ 1,23
B1.18   Despesas                                   Envie, valide e fature novamente as despesas do funcionário                                                                                                                                                                  R$ 1,23
B1.19   Estúdio (Licença)                          Crie e personalize seus apps Odoo                                                                                                                                                                                            R$ 1,23
B1.20   Folgas                                     Alocar folga e seguir solicitações de folga                                                                                                                                                                                  R$ 1,23
B1.21   Recrutamento                               Monitore seu funil de recrutamento                                                                                                                                                                                           R$ 1,23
B1.22   Serviço de Campo (Licença)                 Programe e acompanhe as operações, tempo e material no local                                                                                                                                                                 R$ 1,23
B1.23   Funcionários                               Centralize informações dos funcionários                                                                                                                                                                                      R$ 1,23
B1.24   Reciclagem de dados                        Encontre registros antigos e arquive/delete-os                                                                                                                                                                               R$ 1,23
B1.25   Manutenção                                 Rastreie equipamentos e gerencie solicitações de manutenção                                                                                                                                                                  R$ 1,23
B1.26   Cartão de marketing                        Gerar cartões compartilháveis dinâmicos                                                                                                                                                                                      R$ 1,23
B1.27   Assinatura de Documentos (Licença)         Envie documentos para assinatura online e processe as cópias preenchidas                                                                                                                                                     R$ 1,23
B1.28   Central de Ajuda (Licença)                 Rastreie, priorize e resolva chamados de clientes                                                                                                                                                                            R$ 1,23
B1.29   Assinaturas (Licença)                      Gere faturas recorrentes e administre renovações                                                                                                                                                                             R$ 1,23
B1.30   Qualidade (Licença)                        Controle a qualidade de seus produtos                                                                                                                                                                                        R$ 1,23
B1.31   e-Learning                                 Gerencie e publique uma plataforma de e-Learning                                                                                                                                                                             R$ 1,23
B1.32   Planejamento (Licença)                     Gerencie o cronograma dos seus funcionários                                                                                                                                                                                  R$ 1,23
B1.33   Eventos                                    Publique eventos, venda ingressos                                                                                                                                                                                            R$ 1,23
B1.34   Mensagens                                  Chat, gateway de e-mail e canais privados                                                                                                                                                                                    R$ 1,23
B1.35   Contatos                                   Centralize seus contatos                                                                                                                                                                                                     R$ 1,23
B1.36   PLM – Ciclo de Vida do Produto (Licença)   Gerencie ordens de alteração de engenharia em produtos, listas de materiais                                                                                                                                                  R$ 1,23
B1.37   Calendário                                 Agente reuniões dos funcionários                                                                                                                                                                                             R$ 1,23
B1.38   Redes Sociais (Licença)                    Gerencie suas redes sociais e visitantes do site                                                                                                                                                                             R$ 1,23
B1.39   Avaliações (Licença)                       Avalie seus funcionários                                                                                                                                                                                                     R$ 1,23
B1.40   Frota                                      Gerencie sua frota e acompanhe os custos de veículos                                                                                                                                                                         R$ 1,23
B1.41   Automação de Marketing (Licença)           Crie campanhas de envio em massa automatizadas                                                                                                                                                                               R$ 1,23
B1.42   Chat ao Vivo                               Converse com visitantes do seu site                                                                                                                                                                                          R$ 1,23
B1.43   Compromissos (Licença)                     Permita que as pessoas agendem reuniões em sua agenda                                                                                                                                                                        R$ 1,23
B1.44   Pesquisas                                  Envie suas pesquisas ou compartilhe-as ao vivo                                                                                                                                                                               R$ 1,23
B1.45   Celular (Licença)                          Este módulo é o núcleo do aplicativo Odoo Mobile                                                                                                                                                                             R$ 1,23
B1.46   Reparos                                    Repare produtos danificados                                                                                                                                                                                                  R$ 1,23
B1.47   Controle de Presença                       Monitore a presença de funcionários                                                                                                                                                                                          R$ 1,23
B1.48   Marketing por SMS                          Crie, envie e rastreie SMS                                                                                                                                                                                                   R$ 1,23
B1.49   Código de Barras (Licença)                 Use leitores de código de barras para processar operações logísticas                                                                                                                                                         R$ 1,23
B1.50   Lista de Tarefas                           Organize seu trabalho com memorandos e listas de tarefas                                                                                                                                                                     R$ 1,23
B1.51   Gestão de habilidades                      Gerencie as habilidades, o conhecimento e os currículos de seus funcionários                                                                                                                                                 R$ 1,23
B1.52   VoIP (Licença)                             Faça e receba ligações de dentro do Odoo.                                                                                                                                                                                    R$ 1,23
B1.53   Almoço                                     Processe pedidos de refeições de seus funcionários                                                                                                                                                                           R$ 1,23
B1.54   Vagas de emprego online                    Gerencie seu processo de contratação online                                                                                                                                                                                  R$ 1,23
B1.55   Conector Amazon (Licença)                  Importar pedidos da Amazon e sincronizar as entregas                                                                                                                                                                         R$ 1,23
B1.56   Contratos de funcionários                                                                                                                                                                                                                                               R$ 1,23
B1.57   Licenças                                                                                                                                                                                                                                                               R$ 49,00

                                                     O EVAH Omni é a central de gerenciamento omnichannel baseada na plataforma Chatwoot, integrada ao ecossistema EVAH para oferecer um atendimento unificado, eficiente e supervisionado. Ele possibilita que atendentes humanos assumam o controle das
                                  EVAH Omni                                                                      conversas iniciadas nos canais digitais, garantindo continuidade, qualidade e personalização no relacionamento com o cliente.
                                              Assistente Inteligente de Vendas Automatizado para Humanos. O Evah Assistant é o assistente conversacional com inteligência artificial da solução EVAH. Projetado para operar de forma inteligente e supervisionada, ele atua em duas modalidades complementares —
                                                                                                                                  otimizando processos de atendimento, vendas e suporte com alta adaptabilidade.
                  EVAH Assistant: "Evah Assistant"        Capaz de compreender contextos complexos, aplicar regras de negócio personalizadas e integrar-se a múltiplos sistemas, o Evah Assistant é um agente estratégico no relacionamento com o cliente, promovendo uma experiência fluida e humanizada dentro do
                                                                                                                                                                  ecossistema EVAH.

                               Componente                                                                   Descrição                                                                    Tipo cobrança     Qual custo                            Custos               Valor custo            Req Ref
                                            Os widgets de chat ao vivo do Chatwoot podem ser personalizados com base na sua marca, idioma etc.
                                            - Multilíngue, suporta mais de 10 idiomas
                                            - Continue a conversa por e-mail
C1.1    Live-Chat Adaptával                 - Suporte para emojis e anexos                                                                                                                                                                                              R$ 500,00
                                            - Personalize as cores dos widgets com base na sua marca
                                            - Indicadores de digitação para melhorar a experiência do usuário
                                            - Janela pop-out para mensagens sem distrações
                                            - Crie seu fluxo de automação personalizado com um conjunto de regras simples. Selecione um gatilho no menu suspenso, defina uma ou
                                            várias condições de qualificação e defina as ações desejadas — em minutos.
C1.5    Automações                          - "Escolha acionar um fluxo de automação a partir de três tipos de eventos: “Conversa criada”, “Conversa atualizada” e “Mensagem criada”."                                                                                  R$ 13,56
                                            - Condições são critérios a serem verificados antes da execução de uma ação. O Chatwoot sugere condições a serem definidas com base
                                            no evento que acionou a ação. E oferece a opção de adicionar várias condições.
C1.6    Aplicativos Mobile                  - Gerencie conversas em qualquer lugar: baixar o app via App Store ou Google Store                                                                                                                                          R$ 13,56
                                            - HubSpot: CRM (com ferramentas de marketing, vendas e atendimento)
                                            - Zoho: CRM (com suíte completa de apps empresariais)
                                            - Attio: CRM (focado em organização e colaboração de contatos)
                                            - LeadSquared: CRM (com automação de marketing)
                                            - Shopify: E-commerce (plataforma para loja online)
                                            - WooCommerce: E-commerce (plugin para transformar sites WordPress em lojas online)
                                            - Dialogflow: Plataforma de criação de chatbots e assistentes virtuais com IA
C1.7    Integrações                         - Slack: Plataforma de comunicação e colaboração em equipe                                                                                                                                                                  R$ 13,56
                                            - Google Translate: Serviço de tradução automática de idiomas
                                            - Dyte: Plataforma para integrar vídeo chamadas em apps e sites
                                            - Linear: Ferramenta de gestão de projetos e rastreamento de bugs
                                            - GitHub: Plataforma de hospedagem e controle de versões para código-fonte
                                            - Calendly: Ferramenta para agendamento automático de reuniões
                                            - Cal.com: Plataforma open-source para agendamento de compromissos
                                            - Stripe: Plataforma para processamento de pagamentos online
                                            - Colete informações sobre um contato/conversa antes de iniciar uma conversa com ele, com formulários pré-chat.
                                            - Ative seu formulário pré-chat, ative os campos que deseja mostrar no formulário, adicione texto útil e você estará pronto para publicar!
C1.8    Contexto Ágil instantâneo                                                                                                                                                                                                                                       R$ 13,56
                                            - Não se limite a nomes e e-mails. Colete o máximo de informações necessárias por meio do formulário pré-chat. Basta mapear os campos
                                            do seu formulário pré-chat com os atributos personalizados que você criar na sua conta do Chatwoot.
                                            - Certificados SSL
                                            Obtenha documentação segura com seu domínio personalizado.
                                            - Locais
                                            Torne seus artigos informativos acessíveis a todos.
                                            - Widget de bate-papo ao vivo
                                            Anexe sua central de ajuda ao widget de chat ao vivo com um único clique.
C1.9    Central de Ajuda - EVAH Omni                                                                                                                                                                                                                                    R$ 13,56
                                            - Categorias
                                            Mantenha seus artigos informativos bem organizados e facilmente acessíveis.
                                            - Suporte completo à API
                                            Crie aplicativos personalizados inovadores com nossa API avançada e poderosa.
                                            - Páginas privadas
                                            Forneça acesso restrito e selecionado a páginas específicas.
                                            - Organize facilmente suas conversas com rótulos
                                            - Crie e personalize suas etiquetas
C1.10   Etiquetas                                                                                                                                                                                                                                                       R$ 13,56
                                            - Rotule instantaneamente suas conversas recebidas
                                            - Obtenha uma visão geral de seus rótulos
                                            - Organize seus agentes em equipes
C1.11   Equipes                             - Atribua automaticamente suas conversas a equipes específicas                                                                                                                                                              R$ 13,56
                                            - Análise de equipe
                                            - Anote informações importantes sobre seus contatos
                                            - Adicione notas facilmente, a qualquer momento
C1.12   Notas de Contato                                                                                                                                                                                                                                                R$ 13,56
                                            - Formatação de texto enriquecido
                                            - Exclua-os mais tarde
                                            - Trabalhe em conjunto com sua equipe para resolver as dúvidas dos clientes
                                            - Mude facilmente do chat do cliente para a Nota Privada
C1.13   Notas Privadas                                                                                                                                                                                                                                                  R$ 13,56
                                            - Mencione seus companheiros de equipe
                                            - Formate seu texto, adicione anexos e emojis
                                            - Organize seus contatos em segmentos
C1.14   Segmentos de Contato                - Configure segmentos personalizados em segundos                                                                                                                                                                            R$ 13,56
                                            - Acesse seus segmentos rapidamente
                                            - Informe aos clientes que você não está disponível para responder às perguntas deles
                                            - Defina seu horário de trabalho diário e mensagem de indisponibilidade
C1.15   Horário Comercial                                                                                                                                                                                                                                               R$ 13,56
                                            - Defina o horário comercial para cada caixa de entrada separadamente
                                            - Ajuste seus relatórios de desempenho para o horário comercial
                                            - Rastreie e acompanhe as atividades da conta com facilidade
C1.16   Registros de Autoria                - Rastreamento abrangente: quem, o quê, quando e onde                                                                                                                                                                       R$ 13,56
                                            - Rastreamento personalizado para usuários, contas e muito mais
                                            - Veja o status de suas conversas e agentes em tempo real
                                            - Veja quantas conversas estão abertas no momento
C1.17   Vsualização ao vivo                                                                                                                                                                                                                                             R$ 13,56
                                            - Veja quantos agentes estão online no momento
                                            - Veja quem está participando de quantas conversas atualmente
                                                              Assistente Inteligente de Vendas Automatizado para Humanos. O Evah Assistant é o assistente conversacional com inteligência artificial da solução EVAH. Projetado para operar de forma inteligente e supervisionada, ele atua em duas modalidades complementares —
                                                                                                                                                  otimizando processos de atendimento, vendas e suporte com alta adaptabilidade.
                EVAH Assistant: "Evah Assistant"                          Capaz de compreender contextos complexos, aplicar regras de negócio personalizadas e integrar-se a múltiplos sistemas, o Evah Assistant é um agente estratégico no relacionamento com o cliente, promovendo uma experiência fluida e humanizada dentro do
                                                                                                                                                                                  ecossistema EVAH.

                                Componente                                                                                  Descrição                                                                Tipo cobrança          Qual custo                            Custos               Valor custo            Req Ref
                                                            - Obtenha insights detalhados sobre suas conversas
C1.18   Relatório de Conversa                               - Apresentação de dados fácil de entender                                                                                                                                                                                    R$ 13,56
                                                            - Filtros para ver apenas o que você quer ver
                                                            - Acompanhe o desempenho dos seus agentes com relatórios de atualização automática
C1.19   Relatório do Agente                                 - Apresentação de dados fácil de entender                                                                                                                                                                                    R$ 13,56
                                                            - Filtros para ver apenas o que você quer ver
                                                            - Relatório de saúde das suas conversas, filtrado por rótulos
C1.20   Relatório de Rótulos                                - Apresentação de dados fácil de entender                                                                                                                                                                                    R$ 13,56
                                                            - Filtros para ver apenas o que você quer ver
                                                            - Envie e acompanhe pesquisas de satisfação do cliente no piloto automático
C1.21   Relatórios CSAT                                     - Deixe seus clientes se expressarem com emojis                                                                                                                                                                              R$ 13,56
                                                            - Visualize e baixe seus relatórios CSAT
                                                            - Obtenha insights sobre suas caixas de entrada com relatórios de atualização automática
C1.22   Relatórios de caixa de entrada                      - Apresentação de dados fácil de entender                                                                                                                                                                                    R$ 13,56
                                                            - Filtros para ver apenas o que você quer ver
                                                            - Acompanhe o desempenho de cada uma de suas equipes com relatórios de atualização automática
C1.23   Relatórios de equipe                                - Apresentação de dados fácil de entender                                                                                                                                                                                    R$ 13,56
                                                            - Filtros para ver apenas o que você quer ver

                                                            O EVAH Maestro é o núcleo de automações inteligentes do ecossistema EVAH, utilizando a plataforma open source n8n para criar, gerenciar e executar fluxos complexos que integram múltiplos sistemas, canais e processos empresariais. Seu design modular e
                      EVAH Maestro                          escalável permite que a operação seja automatizada com alta flexibilidade, garantindo agilidade, controle e precisão.

E1.1    Fluxos (Workfows) personalizados                                                                                                                                                                                                                                                 R$ 120,00
E1.2
E1.3
E1.4

                EVAH Hospedagem/Infra
        Atendimento via canal Whatsapp (Evolution API)      - Integra o Evah Assistant ao WhatsApp usando a Evolution API, com suporte a mensagens, envio e recebimento de mídias e automações. É ágil
H1.1                                                                                                                                                                                                                                                                                     R$ 82,20
        (Hospedágem)                                        para implantar, flexível e compatível com diferentes cenários de atendimento, utilizando provedores intermediários.
H1.2    Hospedagem Onpremise ERP                                                                                                                                                                                                                                                         R$ 82,20
H1.3    Hospedagem Onpremise Omni                                                                                                                                                                                                                                                        R$ 82,20
H1.4    Hospedagem Onpremise maestro                                                                                                                                                                                                                                                     R$ 82,20
                                                            - Personalização de fluxos específicos no Typebot para coleta de informações, preenchimento de agendas, validações e outras automações
H1.5    Guidado - Atendimento guiado (Hospedagem Typebot)                                                                                                                                                                                                                                R$ 82,20
                                                            essenciais ao atendimento guiado.
H1.6    Banco de dados (RDS)                                                                                                                                                                                                                                                             R$ 100,00
---

### Arquivo: EVAH –  Proposta Comercial Bira Veículos - Plano de Implantação.md# EVAH –  Proposta Comercial Bira Veículos - Plano de Implantação

---

                                                                                             EVAH – Vendas Inteligentes Automatizadas e Humanizadas

                       Módulo / funcionalidade                                                    Descrição Atividade                                Preço Implantação        Hospedágem            Preço Suporte   Status   MVP
1   EVAH Assistent Evah Assistant
                                                                                                                                                                         Gratuita (Evolution API)
                                                                       - Criar uma instancia na AWS para implantar a EvolutionAPI
                                                                                                                                                                         ou API oficial da Meta =
                                                                       - Configurar a instancia (docker, swarm, portainer, traefik...)
    API Integração com WhatsApp                                                                                                                                          exige número verificado
                                                                       - Implanta a Stack via yml
                                                                                                                                                                             + cobrança por
                                                                       - Criar e registrar um subdominio unico para disponibilizar a API
                                                                                                                                                                                conversa
    API Integração com Instagran
    API Integração com Telegran                                                                                                                                              Gratuito/ OBS:
    API Integração com Facebook                                                                                                                                              Gratuito/ OBS:
    API Integração com WebChat
                                                                        Permite que o Evah Assistant funcione sob um subdomínio do cliente, com SSL e
    Configuração vinculada ao dominio do cliente                       identidade visual personalizada. Requer configuração de DNS (CNAME ou
                                                                                                        A record).
                                                                       Conecta o Evah Assistant a serviços avançados de IA, como OpenAI (ChatGPT),
                                                                         Google Gemini, IBM Watson e outros. Permite geração contextual de
    Integração com API de inteligência Artificial (Custos variaveis)
                                                                       respostas, análise de sentimentos, interpretação de dados estruturados e
                                                                           não estruturados, além de automações dinâmicas e inteligentes.
    Integração com Google calendar
    Integração com Google Drive
    Implantação do Typebot (Atendimento guiado)
                                                                         Consulta e inserção de produtos, leads, dados financeiros e outros
    Integração com EVAH ERP para consulta de produtos                  módulos via API do ERP EVAH, com segurança, controle de acesso e logs
                                                                                                   para auditoria.
    Desenvolvimento de fluxos de negócio
                                                                       Personalização de acordo com a atividade comercial do cliente (imobiliaria,
    Personalização do Assistente
                                                                           escritorios de serviços e consultoria diversas, venda de automoveis
                                                                        Processo automatizado para converter e transcrever diferentes formatos
                                                                       de mensagens recebidas, garantindo acessibilidade, melhor entendimento
                                                                                            e agilidade no atendimento. Inclui:

                                                                         Áudio para texto: reconhecimento automático da fala para transformar
                                                                                  mensagens de voz em texto legível e pesquisável.
    Conversão e Transcrição de Mensagens
                                                                       Texto para áudio: síntese de voz para transformar mensagens escritas em
                                                                                 áudio, facilitando o consumo em diferentes contextos.

                                                                       Transcrição de PDFs: extração de texto de documentos PDF para consulta
                                                                                     rápida e integração com fluxos automatizados.

                                                                         Identificação e transcrição de imagens: uso de OCR (reconhecimento
                                                                        óptico de caracteres) para extrair texto de imagens enviadas pelo cliente.

2   EVAH ERP (odoo, outro)
    Instalação do Odoo                                                                                                                                                                               R$ 4.000,00
    Implatação do Odoo
    Treinamento
3   EVAH Omni (chatwoot)

4   EVAH Connect

5   EVAH Conductor

6   EVAH Code
    Criação de Componentes Exclusivos
    Integrações com Sistemas Legados ou Proprietários
    Extensão de Fluxos e Automações Complexas
    Personalização de Interface e Experiência Conversacional
    Criação de APIs Customizadas
    Suporte a Projetos Especiais e Provas de Conceito
    Gerenciamento de Ciclo de Vida do Código
---

### Arquivo: EVAH Framework Modular.md# 📦 EVAH – Framework Modular para Atendimento e Gestão Comercial

## 🧱 O que é o EVAH?

`EVAH` é um **framework modular** criado para transformar o modo como empresas capturam, atendem e convertem seus leads. 
Ele serve como base para soluções personalizadas de **automação, atendimento e gestão comercial**, adaptável ao porte e maturidade do negócio.

> Com o EVAH, o negócio começa enxuto e cresce com inteligência, mantendo eficiência, escala e flexibilidade.

---

## 🤖 Evah Assistant – O Chatbot Inteligente do EVAH

- `Evah Assistant` é o **assistente conversacional inteligente** desenvolvido sobre o framework EVAH.
- Atua como linha de frente no atendimento:
  - Captura de leads
  - Qualificação automatizada
  - Agendamento de visitas
  - Direcionamento para atendimento humano
- Pode ser utilizado:
  - ✅ Como **módulo do EVAH**
  - ✅ Como **solução independente**, ideal para quem quer só automatizar atendimento

---

## 🧩 Estrutura Modular do Framework

| Módulo         | Descrição                                                                  |
|----------------|----------------------------------------------------------------------------|
| `EVAH (core)`  | Lógica de negócio, orquestração de dados e integração entre componentes    |
| `Evah Assistant`        | Chatbot inteligente integrado com Typebot, n8n e APIs externas             |
| Integrações    | Conexões com ERP, WhatsApp, site, redes sociais, formulários               |
| Automações     | Agendamentos, notificações, propostas, CRM, fluxo de vendas                |

---

## 🎯 Objetivo do Projeto

Entregar uma **solução vendável, funcional e escalável** nas mãos do vendedor. 
O framework EVAH permite montar soluções sob medida para resolver as dores reais do processo comercial.

---

## ✅ O que o MVP precisa ter para ser considerado vendável?

- Nome e identidade clara (`EVAH` como framework, `Evah Assistant` como exemplo aplicado)
- Demonstração funcional que mostre valor imediato
- Capacidade de modularização (usar só o que o cliente precisa)
- Resolução de problemas reais (ver abaixo)

---

## 🚨 Dores que o EVAH resolve (M. Aversão)

### Ineficiências comuns:
- ❌ Falta de controle no atendimento ao cliente
- ❌ Gestão ineficiente dos vendedores
- ❌ Atendimento limitado a horário comercial
- ❌ Ausência de automação e personalização
- ❌ Sem estrutura de funil ou oportunidades

### Barreiras à conversão:
- 🟥 Leads não são capturados
- 🟥 Respostas demoram ou não existem
- 🟥 Atendimento sem qualidade
- 🟥 Falta de follow-up e recuperação de leads
- 🟥 Não há histórico das interações
- 🟥 Comunicação não é registrada ou reaproveitada

---

## 🎥 Demonstração do Produto/Solução

### Exemplo com `Evah Assistant` (chatbot):
1. Atendimento inicial humanizado
2. Qualificação automática do lead
3. Sugestão de horários disponíveis
4. Agendamento e confirmação automática
5. Integração com CRM e acompanhamento

---

## 🔧 Backlog de Entrega

### 📌 Site institucional
- [ ] Missão, visão e valores
- [ ] Página "Vender"
- [ ] Planos e pacotes da solução com CTA claro

### 📌 MVP funcional
- [ ] Gestão mínima de leads
- [ ] Fluxo completo de atendimento
- [ ] Notificações básicas (som, push, e-mail)

---

## 📉 Pontos de melhoria na apresentação atual

- ⚠️ Falta de site estruturado
- ⚠️ Ausência de identidade visual (cartão, banner, etc.)
- ⚠️ Solução ainda sem apresentação oficial completa (benefícios + recursos)

---

## 🧠 Observação Estratégica

> O EVAH é pensado para **crescer com o cliente**: 
Empresas podem começar com um módulo como o `Evah Assistant` e, conforme amadurecem, escalar para soluções mais completas. 
Isso reduz barreiras de entrada, acelera a implementação e aumenta a retenção no longo prazo.

---

- ERP Odoo;

- Chatwoot: Gestor de atendimento

- Evah Assistant: Chatboot com atendimento guiado e com inteligencia artificial de "n" possibilidades- recepcionista, agendador, consultor e por ai vai.

- Evolution API: Funcionara como integrador ao whatsapp basicamente

- Typebot: é uma plataforma no-code/low-code para criar conversas interativas em formato de bot, que você pode integrar facilmente em sites, apps, WhatsApp, CRMs, APIs, n8n e muito mais.

- Automações: envolvendo n8n;

- Personalização de acordo com cada cliente para cada segmento
___

Fazer um benchmark entre a EVAH e possíveis concorrentes da Dobem com soluções semelhantes
---



