# VIAH – Vendas Inteligentes Automatizadas e Humanizadas

## Framework Modular para Atendimento e Gestão Comercial

## *Framework \=  Quadro de ferramentas, funcionalidades genéricas para serem implementadas em um negócio específico.*

## 1\. Introdução

O **VIAH** é um framework modular que integra sistemas de atendimento, automação e gestão comercial, oferecendo uma solução robusta em um ecossistema unificado e escalável. Seus módulos trabalham juntos para suportar automações baseadas em fluxos pré-definidos e integrar diversas ferramentas de mercado, garantindo maior controle operacional, além de proporcionar uma experiência humanizada ao cliente com o uso das melhores inteligências artificiais disponíveis.

#### **Principais módulos:**

    • **VIAH Assistent AIVAH** – Assistente Inteligente de Vendas Automatizado para Humanos.  
    • **VIAH ERP** – Sistemas administrativos e financeiros  
    • **VIAH Omni** – Central de Gerenciamento Omnichannel de Atendimento  
    • **VIAH Connect** – Módulo de integração que conecta canais externos, como WhatsApp, e sistemas externos ao ecossistema **VIAH**  
    • **VIAH Maestro** – Orquestrador de automações inteligentes utilizando n8n (a ferramenta que automatiza o processo).  
    • **VIAH Code** – Serviços de desenvolvimento personalizados para criar regras de negócio específicas para cada negócio via APIs, banco de dados e webapp, entre outros.

## **2\. Módulos**

### **2.1 VIAH Assistent AIVAH Assistente Inteligente de Vendas Automatizado para Humanos.**

O **AIVAH** é o assistente conversacional com inteligência artificial da solução **VIAH**. Projetado para operar de forma inteligente e supervisionada, ele atua em duas modalidades complementares — otimizando processos de atendimento, vendas e suporte com alta adaptabilidade.  
Capaz de compreender contextos complexos, aplicar regras de negócio personalizadas e integrar-se a múltiplos sistemas, o **AIVAH** é um agente estratégico no relacionamento com o cliente, promovendo uma experiência fluida e humanizada dentro do ecossistema **VIAH**.

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
  Realiza a transição para atendimento humano mantendo o histórico, o contexto e os dados coletados, seja via VIAH Omni ou plataforma integrada.

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
  Um único AIVAH pode desempenhar múltiplos papéis de forma modular, alternando comportamentos conforme horário, contexto ou setor da empresa.

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

### **2.2 VIAH Omni – Central de Gerenciamento Omnichannel de Atendimento (Chatwoot)**

O **VIAH** Omni é a central de gerenciamento omnichannel baseada na plataforma Chatwoot, integrada ao ecossistema **VIAH** para oferecer um atendimento unificado, eficiente e supervisionado. Ele possibilita que atendentes humanos assumam o controle das conversas iniciadas nos canais digitais, garantindo continuidade, qualidade e personalização no relacionamento com o cliente.

#### Funcionalidades Principais:

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
  * APIs abertas para integração com módulos VIAH, ERP e CRM  
  * Webhooks para captura de eventos e automações avançadas  
  * Suporte para plugins e extensões customizadas

### **2.3 VIAH Connect – Módulo de integração que conecta canais**

O **VIAH** Connect é o módulo responsável por integrar canais externos, como WhatsApp, e sistemas externos ao ecossistema **VIAH**, utilizando a Evolution API. Esta integração permite a comunicação fluida e sincronizada entre plataformas, centralizando o atendimento e otimizando processos.

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

### **2.4 VIAH Maestro – Orquestrador de automações inteligentes utilizando n8n**

O **VIAH Conductor** é o núcleo de automações inteligentes do ecossistema **VIAH**, utilizando a plataforma open source **n8n** para criar, gerenciar e executar fluxos complexos que integram múltiplos sistemas, canais e processos empresariais. Seu design modular e escalável permite que a operação seja automatizada com alta flexibilidade, garantindo agilidade, controle e precisão.

#### Funcionalidades Principais

* **Construção Visual de Workflows**  
  Ambiente intuitivo para montar fluxos de automação através de uma interface drag-and-drop, sem necessidade de programação avançada.

* **Integração Nativa com Sistemas e APIs**  
  Conexão direta com ERP (como Odoo), CRM, bancos de dados, ferramentas de comunicação (WhatsApp via VIAH Connect), e serviços externos via APIs REST e Webhooks.

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

### **2.5 VIAH Code – Serviços de desenvolvimento personalizados**

O módulo **VIAH Code** é responsável por atender demandas específicas que não se enquadram em soluções prontas do ecossistema **VIAH**. Atua como uma camada de extensão flexível, oferecendo serviços sob medida para personalização, automação avançada e integração de sistemas legados ou proprietários.

#### Funcionalidades principais

##### 🔹 Criação de Componentes Exclusivos

* Desenvolvimento de funcionalidades específicas para atender requisitos únicos do cliente, respeitando os padrões e diretrizes do VIAH.

##### 🔹 Integrações com Sistemas Legados ou Proprietários

* Conexão de ERPs, CRMs, bancos de dados, ou APIs internas com os módulos do VIAH, utilizando protocolos seguros e escaláveis.

##### 🔹 Extensão de Fluxos e Automações Complexas

* Implementação de rotinas ou processos que exigem lógica avançada, incluindo manipulação de dados, cálculos personalizados ou regras de negócio complexas.

##### 🔹 Personalização de Interface e Experiência Conversacional

* Ajustes visuais ou de comportamento dos assistentes e interfaces, adaptando a experiência conforme a identidade da empresa ou público-alvo.

##### 🔹 Criação de APIs Customizadas

* Desenvolvimento de APIs RESTful para facilitar a comunicação entre o VIAH e sistemas externos que não possuem conectores diretos.

##### **🔹** Suporte a Projetos Especiais e Provas de Conceito

* Execução de projetos exploratórios, integrações pontuais e protótipos sob demanda, com ciclos curtos de entrega e validação.

##### **🔹 Gerenciamento de Ciclo de Vida do Código**

* Controle de versões, testes automatizados e boas práticas de deploy, garantindo a estabilidade e evolução contínua das personalizações.

###  **2.6 VIAH ERP – Sistemas administrativos e financeiros**

O VIAH ERP é um módulo opcional de gestão administrativa, financeira e operacional. Totalmente integrado ao ecossistema VIAH, oferece funcionalidades robustas e modulares para empresas que não possuem ou desejam modernizar seu sistema atual.

**Importante:** Caso o cliente já possua um ERP próprio, não há qualquer impedimento. O **VIAH** integra-se a sistemas externos por meio de conectores nativos ou personalizados via Evolution API.

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
