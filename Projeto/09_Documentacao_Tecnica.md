# 📚 DOCUMENTAÇÃO TÉCNICA

## 📋 Índice
- [Guias de Implementação](#guias-de-implementação)
- [APIs e Integrações](#apis-e-integrações)
- [Casos de Uso](#casos-de-uso)
- [Troubleshooting](#troubleshooting)

---

## 📖 Guias de Implementação

### EVAH – Vendas Inteligentes Automatizadas e Humanizadas

**Framework Modular para Atendimento e Gestão Comercial**

#### Introdução

**Principais módulos:**
- **EVAH Assistent Evah Assistant** – Assistente Inteligente de Vendas Automatizado para Humanos
- **EVAH ERP** – Sistemas administrativos e financeiros
- **EVAH Omni** – Central de Gerenciamento Omnichannel de Atendimento
- **EVAH Connect** – Módulo de integração que conecta canais externos, como WhatsApp, e sistemas externos ao ecossistema **EVAH**
- **EVAH Conductor** – Orquestrador de automações inteligentes utilizando n8n
- **EVAH Code** – Serviços de desenvolvimento personalizados para criar regras de negócio específicas para cada negócio via APIs, banco de dados e webapp, entre outros

#### Arquitetura

O **EVAH** é estruturado em módulos independentes que se comunicam por meio de APIs e conectores inteligentes, formando um ecossistema flexível, escalável e altamente integrável. Essa arquitetura permite personalização por cliente, automação de processos e gestão unificada de atendimento e operações comerciais.

**Visão Geral do Fluxo:**

O funcionamento do **EVAH** é baseado em uma sequência inteligente de eventos que conecta clientes, automações, atendimento humano e sistemas de gestão:

- **Entrada do cliente:** Interações iniciadas via WhatsApp ou site são recebidas pelo **EVAH Link** (antigo Evolution API)
- **Condução conversacional:** O **EVAH Chat** (antigo Typebot) guia o cliente por fluxos automatizados
- **Respostas inteligentes:** Quando necessário, o **EVAH Evah Assistant** assume o diálogo com IA avançada
- **Automação de tarefas:** O **EVAH Conductor** (n8n) executa ações como agendamentos ou notificações
- **Atendimento humano (opcional):** A conversa pode ser transferida para o **EVAH Omni** (Chatwoot)
- **Registro e gestão:** Todas as informações são integradas ao **EVAH ERP** (Odoo), garantindo controle operacional

### Checklist de Implantação do Evah Assistant

#### 1. Implantação API Integração com WhatsApp
**Descrição:** Configuração e autenticação de canal oficial via API (como Evolution API, Meta Official ou Z-API). Inclui webhook, testes e validação do fluxo de mensagens.  
**Observações:** Pode incluir verificação de número comercial e template de mensagens.  
**Sugestão de preço:** R$ 600 – R$ 1.200 (não inclui custo mensal da API)

#### 2. Implantação API Integração com Instagram
**Descrição:** Configuração da API oficial do Meta para integração com Instagram Direct Messages. Inclui autenticação, webhooks e validação de fluxos.  
**Sugestão de preço:** R$ 400 – R$ 800

#### 3. Implantação API Integração com Telegram
**Descrição:** Configuração da API oficial do Telegram para integração com mensagens. Inclui bot setup, webhooks e validação.  
**Sugestão de preço:** R$ 300 – R$ 600

#### 4. Implantação API Integração com Facebook
**Descrição:** Configuração da API oficial do Meta para integração com Facebook Messenger. Inclui autenticação e webhooks.  
**Sugestão de preço:** R$ 400 – R$ 800

#### 5. Implantação API Integração com WebChat
**Descrição:** Configuração do widget de chat para sites. Inclui integração com Chatwoot ou solução customizada.  
**Sugestão de preço:** R$ 500 – R$ 1.000

#### 6. Configuração vinculada ao domínio do cliente
**Descrição:** Configuração de DNS, SSL e subdomínios para serviços do cliente. Inclui Traefik, certificados Let's Encrypt e validação.  
**Sugestão de preço:** R$ 300 – R$ 600

#### 7. Integração com API de Inteligência Artificial (Custos variáveis)
**Descrição:** Configuração de integração com OpenAI (ChatGPT), Google Gemini ou IBM Watson. Inclui setup de credenciais, rate limiting e monitoramento de custos.  
**Observações:** Custos variáveis conforme uso (tokens)  
**Sugestão de preço:** R$ 200 – R$ 500 (setup) + custos variáveis

#### 8. Integração com Google Calendar
**Descrição:** Configuração da API do Google Calendar para agendamentos automáticos. Inclui OAuth, permissões e validação de fluxos.  
**Sugestão de preço:** R$ 400 – R$ 800

#### 9. Implantação do Typebot (Atendimento guiado)
**Descrição:** Instalação e configuração do Typebot para fluxos conversacionais guiados. Inclui criação de fluxos básicos, hospedagem e integração com canais.  
**Sugestão de preço:** R$ 800 – R$ 1.500

#### 10. Integração com EVAH ERP para consulta de produtos
**Descrição:** Desenvolvimento de integração entre assistente e ERP (Odoo) para consultas de produtos, estoque e informações comerciais em tempo real.  
**Sugestão de preço:** R$ 1.000 – R$ 2.000

#### 11. Desenvolvimento de fluxos de negócio
**Descrição:** Mapeamento e desenvolvimento de fluxos conversacionais específicos do negócio do cliente. Inclui análise de processos, criação de jornadas e validação.  
**Sugestão de preço:** R$ 2.000 – R$ 5.000 (conforme complexidade)

#### 12. Personalização do Assistente
**Descrição:** Treinamento do assistente com dados específicos do cliente, ajuste de prompts, personalização de respostas e integração com regras de negócio.  
**Sugestão de preço:** R$ 1.500 – R$ 3.000

**Total Estimado de Implantação:** R$ 7.400 – R$ 17.800 (sem custos variáveis de APIs)

### Funcionalidades do Typebot

**Principais funcionalidades:**

#### Construção de Fluxos
- Editor **drag-and-drop** para criar conversas sem precisar programar
- Blocos de texto, botões, múltipla escolha e campos de input
- Captura de informações do usuário (nome, email, telefone etc.)
- Condições e ramificações (lógica condicional para personalizar o fluxo)

#### Integrações
- Integração nativa com **WhatsApp**, **Telegram** e **Messenger**
- Embeds em sites (widget flutuante ou página inteira)
- Integração com **Google Sheets**, **Webhooks**, **APIs externas**
- Conexão com ferramentas como **Zapier**, **Make** e **n8n**

#### Automação e Personalização
- Uso de **variáveis** para armazenar respostas e personalizar a conversa
- Condições lógicas (se/senão) para adaptar a jornada do usuário
- Redirecionamento entre blocos de forma dinâmica
- Respostas rápidas e botões interativos

#### Coleta de Dados
- Formulários conversacionais (lead forms em formato de chat)
- Validação de campos (ex: email válido, número de telefone)
- Armazenamento de dados para exportação

#### Design e Experiência
- Personalização de cores, fontes e estilo do chatbot
- Emojis, imagens, vídeos, GIFs e carrosséis
- Suporte a mensagens de áudio e mídia em alguns canais

#### Gerenciamento e Publicação
- Hospedagem automática em links do Typebot
- Publicação como widget em sites (iframe ou script)
- Conexão com domínios próprios
- Monitoramento de respostas e coleta de métricas básicas

## 🔗 APIs e Integrações

### Integração n8n com Chatwoot

**É possível integrar o n8n com o Web Chat do Chatwoot** através de webhooks e API pública.

#### Receber mensagens do Web Chat no n8n

1. Vá até **Chatwoot > Settings > Account Settings > Webhooks**
2. Cadastre a **URL do webhook** do seu fluxo no n8n (`https://seu-n8n/webhook/nome-do-fluxo`)
3. Toda nova mensagem, evento de conversa, etc., será enviada para o n8n no formato JSON
4. No n8n, você pode usar o nó `Webhook` para capturar esses dados e:
   - Processar com IA
   - Gravar em banco de dados ou CRM
   - Acionar automações (e.g. N8N + GPT + ERP)

#### Responder via Web Chat a partir do n8n

Use a rota da API:
```http
POST /api/v1/accounts/{account_id}/conversations/{conversation_id}/messages
```

Com um corpo como:
```json
{
  "content": "Sua resposta aqui",
  "message_type": "outgoing"
}
```

Autentique com o token do seu agente (ou com token de API).

#### Fluxo típico de integração

1. **Usuário envia mensagem no Web Chat**
2. Chatwoot dispara webhook → **n8n recebe**
3. n8n interpreta (com IA ou lógica)
4. n8n envia resposta via **API do Chatwoot** → **usuário vê no Web Chat**

### Nome do nó Evolution API no n8n

No **n8n**, não existe oficialmente um nó chamado **"evolution"**. 

**Soluções:**
- Use **HTTP Request** quando você integra via REST
- Ou use um **nó customizado** caso alguém tenha criado um pacote específico
- O nó Evolution API pode ser um *community node* (nó da comunidade) que precisa ser instalado separadamente

**Para restaurar/instalar:**
1. Verifique se o *Community Nodes* está ativado/configurado no seu n8n
2. Há geralmente uma aba em **Settings → Community Nodes**
3. Instale o pacote da Evolution API se disponível

### Enviar mensagem para Typebot

**URL de exemplo:**
```
https://typebotapi.bira.dev.biraveiculos.com.br/api/v1/typebots/cm868vsm300058qn4jof7or0b/preview/startChat
```

**Método:** POST

**Headers:**
- `Content-Type: application/json`
- Pode ser que precise de algum token ou autenticação, dependendo da API

**Body (exemplo):**
```json
{
  "message": "Olá, quero iniciar uma conversa"
}
```

**Exemplo em cURL:**
```bash
curl -X POST "https://typebotapi.bira.dev.biraveiculos.com.br/api/v1/typebots/cm868vsm300058qn4jof7or0b/preview/startChat" \
-H "Content-Type: application/json" \
-d '{"message":"Olá, quero iniciar uma conversa"}'
```

**Exemplo em Python (requests):**
```python
import requests

url = "https://typebotapi.bira.dev.biraveiculos.com.br/api/v1/typebots/cm868vsm300058qn4jof7or0b/preview/startChat"
payload = {
    "message": "Olá, quero iniciar uma conversa"
}
headers = {
    "Content-Type": "application/json"
}

response = requests.post(url, json=payload, headers=headers)
print(response.status_code)
print(response.json())
```

### Receber áudio no Typebot

**Problema:** Atualmente, **o Typebot não possui suporte nativo para entrada de áudio** — ele trabalha com mensagens de texto, botões, formulários, entre outros componentes interativos, mas **não tem um componente para interpretar ou processar áudios diretamente**.

**Solução alternativa:** Transcrever o áudio antes de enviar ao Typebot

**Fluxo recomendado:**
1. **Usuário envia áudio via WhatsApp**
2. **Evolution API 2 recebe o áudio** (você pode capturar a URL do arquivo de áudio via webhook)
3. **Você usa uma API de transcrição de voz** (como a **Whisper API da OpenAI**, ou Google Speech-to-Text) para converter o áudio em texto
4. **O texto transcrito é enviado para o Typebot** como se fosse a mensagem do usuário

**Ferramentas para transcrição:**
- **Whisper API da OpenAI:** Endpoint `https://api.openai.com/v1/audio/transcriptions`
- **Google Cloud Speech-to-Text:** Mais complexo de configurar, mas suporta múltiplos idiomas

**Integração com N8N:**
Você pode montar esse fluxo com:
- Webhook do Evolution recebendo o áudio
- Baixar o áudio (via HTTP Request)
- Passar para o Whisper
- Obter o texto transcrito
- Enviar para o Typebot via Webhook ou API de entrada

### Tratamento de input monetário

**Algoritmo JavaScript para tratar entradas diversas de valores monetários:**

```javascript
function parseValor(input) {
  if (!input || typeof input !== 'string') return 0.00;

  // Remove símbolos de moeda, espaços, letras e outros caracteres
  let cleaned = input.replace(/[^0-9.,]/g, '').trim();

  // Se houver mais de uma vírgula e ponto, assume-se que vírgula é decimal (formato BR)
  const hasComma = cleaned.includes(',');
  const hasDot = cleaned.includes('.');

  if (hasComma && hasDot) {
    // Assume formato brasileiro: milhar com ponto e decimal com vírgula → 1.234,56
    cleaned = cleaned.replace(/\./g, '').replace(',', '.');
  } else if (hasComma && !hasDot) {
    // Apenas vírgula → troca por ponto (decimal)
    cleaned = cleaned.replace(',', '.');
  } else if (hasDot && !hasComma) {
    // Apenas ponto → já está no formato certo
    // Ex: 1234.56
  }

  // Converte para número float
  const number = parseFloat(cleaned);
  
  // Retorna com duas casas decimais
  return isNaN(number) ? 0.00 : parseFloat(number.toFixed(2));
}
```

**Exemplos de entradas tratadas:**
- `"R$ 123,45"` → 123.45
- `"123.45"` → 123.45
- `"1.234,56"` → 1234.56
- `"USD 1,234.56"` → 1234.56
- `"  1.234,56  "` → 1234.56
- `"1234"` → 1234.00

## 💡 Casos de Uso

### Agente Orquestrador no n8n

**Conceito:** Criar um **agente de IA orquestrador no n8n** que coordena outros agentes especializados (como agendamento, pagamento, atendimento, etc.)

**Estrutura Recomendada (Arquitetura Modular):**

#### Agente Orquestrador (Master Agent)
- Interpreta o input do usuário (via IA)
- Identifica a intenção (ex: "Quero agendar uma reunião")
- Aciona o agente especializado correspondente

#### Agentes Especializados
Cada um é um workflow separado no n8n:
- `AgenteAgenda`: interage com Google Calendar
- `AgentePagamentos`: executa cobranças via Stripe, Mercado Pago, etc.
- `AgenteCRM`: registra dados no CRM
- `AgenteProdutos`: lista e filtra produtos de uma base

**Como Montar no n8n (Passo a Passo):**

1. **Entrada do Usuário**
   - Use um trigger como: **Webhook** (se for via WhatsApp, Telegram, site, etc.)

2. **ChatGPT ou OpenAI Node (Interpretação da Intenção)**
   - Pergunte: _"Qual a intenção do usuário?"_
   - Exemplo de prompt:
     ```
     Usuário disse: "{{input}}"
     Identifique a intenção com base na lista:
     - agendar_visita
     - fazer_pagamento
     - consultar_produtos
     - outro
     Responda apenas com a intenção.
     ```

3. **Switch Node (Roteamento por Intenção)**
   - Com base na resposta da IA, direcione para o workflow do agente especializado correspondente

4. **Execução do Agente Especializado**
   - Cada agente especializado executa sua tarefa específica
   - Retorna resultado para o orquestrador

5. **Resposta Final**
   - Orquestrador consolida resultados e retorna resposta ao usuário

### Assistente de Produtos com JSON

**Objetivo:** Desenvolver um assistente que seja capaz de receber uma lista em JSON de produtos e identificar se dentro do item da lista existe o produto que o cliente pediu.

**Funcionalidades:**
1. Receber uma lista de produtos (como carros ou qualquer outro item) em formato JSON
2. Entender o que o cliente está buscando (ex: "tem Corolla 2022?")
3. Verificar se há correspondência na lista
4. Gerar uma resposta amigável, dizendo se há ou não, e listando os produtos correspondentes de forma agradável

**Estrutura JSON (exemplo de entrada):**
```json
[
  {
    "marca": "Toyota",
    "modelo": "Corolla",
    "ano": 2022,
    "preco": "R$ 95.000",
    "cor": "Preto"
  },
  {
    "marca": "Honda",
    "modelo": "Civic",
    "ano": 2021,
    "preco": "R$ 89.000",
    "cor": "Prata"
  }
]
```

**Lógica de busca:**
- Comparar termos da consulta do cliente com atributos dos produtos
- Retornar produtos correspondentes de forma formatada e amigável
- Informar quando não há correspondências

## 🔧 Troubleshooting

### Erro de DNS no webhook

**Problema:** Evolution API não consegue enviar webhook para o servidor.

**Sintomas:**
- Erro de conexão no log da Evolution API
- Mensagem: "Aguardando X segundos antes da próxima tentativa"
- URL do webhook não responde

**Soluções:**
1. Verificar se o DNS do webhook está configurado corretamente
2. Verificar se o servidor está acessível publicamente
3. Verificar certificados SSL se estiver usando HTTPS
4. Verificar firewall e security groups
5. Verificar se o serviço que recebe o webhook está rodando

### Erros na stack Docker

**Problemas comuns:**
- Erro de digitação em variável de ambiente (ex: caracteres inválidos)
- Volume duplicado e conflitante
- Configurações de rede incorretas
- Variáveis de ambiente mal formatadas

**Soluções:**
- Revisar todas as variáveis de ambiente
- Verificar volumes declarados
- Validar sintaxe YAML
- Testar conexões de rede

### Análise de stack n8n

**Configuração típica:**
- Versão: n8n 1.110.1
- Banco de dados: PostgreSQL (RDS)
- Redis: Para filas (Bull)
- Modo de execução: Queue
- Community packages: Habilitado

**Variáveis importantes:**
- `N8N_ENCRYPTION_KEY`: Chave de criptografia
- `N8N_HOST`: Host do n8n
- `WEBHOOK_URL`: URL base para webhooks
- `EXECUTIONS_MODE`: Modo de execução (queue ou regular)
- `N8N_COMMUNITY_PACKAGES_ENABLED`: Habilitar pacotes da comunidade

### Comparação n8n e LangGraph

**n8n:**
- Ferramenta de orquestração / automação de workflows
- Interface visual ("drag & drop") para construir fluxos
- Permite inserir código personalizado (JS ou Python)
- Pode ser auto-hospedada (self-hosted) ou em nuvem gerenciada
- Possui integração nativa com modelos de IA

**LangGraph:**
- Biblioteca/ferramenta orientada para fluxos de trabalho com IA
- Muito voltada a programadores ou equipes com conhecimentos técnicos
- Mais flexibilidade para workflows dinâmicos, agentes com múltiplos passos, estado persistente

**Quando usar cada um:**
- **n8n:** Quando precisa de interface visual, integração com múltiplos sistemas, automação geral
- **LangGraph:** Quando precisa de agentes de IA complexos, estado persistente, lógica de decisão avançada

### Deploy JHipster ECS Fargate

**Recursos AWS provisionados via Terraform:**
- VPC: aws_vpc.main
- Internet Gateway: aws_internet_gateway.igw
- Subnet pública: aws_subnet.public_a
- Route table: aws_route_table.public
- Security group: aws_security_group.ec2_sg
- EC2 (swarm manager): aws_instance.swarm_manager
- Elastic IP: aws_eip.swarm_eip

**Stacks rodando:**
- Traefik (stack: traefik)
- Portainer (stack: portainer)

**Adicionar mais stacks:**
- É possível adicionar novas stacks utilizando o Portainer e via Terraform
- Usar Portainer API via Terraform para criar e gerenciar stacks
- Ou usar Portainer como interface manual para testes rápidos

### Ajuste de relacionamentos JDL

**Problema:** Precisar colocar o atributo da entidade em vez do id no relacionamento.

**Solução:** No JDL do JHipster, você pode especificar campos de exibição nos relacionamentos usando a sintaxe apropriada.

---

## 📋 CASO DE USO: PLANEJAMENTO DO ASSISTENTE VIRTUAL EVAH ASSISTANT (BIRABOT) - BIRA VEÍCULOS

### Visão Geral

Evah Assistant, apresentado aos clientes como **BiraBot**, é um assistente virtual desenvolvido para realizar **atendimento automatizado em empresas de venda de veículos**, com foco em:

- Atendimento inicial com boas-vindas
- Entendimento do interesse do cliente
- Consulta de veículos disponíveis
- Registro e atualização de leads no CRM (Odoo)
- Agendamento de visitas
- Interpretação de mídia (áudio, imagem, link)
- Consulta baseada em links (web scraping)

### Objetivos do Assistente

#### Comunicação Inicial
- Detectar e responder a saudações como "bom dia", "boa tarde", "olá", etc.
- Apresentar-se como BiraBot e explicar sua função

#### Coleta de Interesse do Cliente
- Identificar tipo de veículo desejado
- Extrair informações como:
  - Marca / modelo
  - Tipo (SUV, hatch, sedan...)
  - Ano mínimo e máximo
  - Faixa de preço

#### Consulta de Veículos
- Integrar com agente que consulta banco de dados
- Apresentar resultados baseados nos filtros coletados

#### Registro e Qualificação de Lead
- Integrar com CRM Odoo para:
  - Criar lead no início do atendimento
  - Atualizar lead à medida que mais dados são fornecidos

#### Agendamento de Visita
- Perguntar disponibilidade do cliente
- Registrar data e hora sugerida
- (Futuramente: integrar com agenda de vendedores)

#### Interpretação Multimídia
- **Áudio:**
  - Transcrever voz em texto
  - Passar texto para o orquestrador
- **Imagem:**
  - Extrair dados visuais (modelo, tipo, cor)
  - Consultar no banco veículos semelhantes
- **Link (Web Scraping):**
  - Extrair dados de anúncios (OLX, Webmotors, etc.)
  - Realizar consulta no banco com base nesses dados

#### Memória e Contexto
- Usar memória (ex: Zep) para manter o histórico do cliente
- Ex: "Quero um carro de 2022" + depois "quero que seja SUV" → entender que busca é SUV de 2022

### Arquitetura Modular no N8N

#### Fluxo Geral:
1. **1_Main_EntradaMensagem** – Entrada de texto, áudio ou imagem
2. **2_TratamentoMensagem** – Converte áudio, texto, imagem em texto limpo
3. **3_Orquestrador** – Detecta a intenção do cliente
4. **4_RoteadorDeAgentes** – Direciona para o agente correto com base na intenção
5. **Agentes Específicos:**
   - 5_AgenteBoasVindas
   - 6_AgenteConsultaVeiculos
   - 7_AgenteWebScraping
   - 8_AgenteAgendamento
   - 9_AgenteCRM
   - 10_AgenteDesconhecido (Fallback)

#### Módulos e Funções

**1. Entrada**
- Recebe mensagem
- Redireciona para tratamento

**2. Tratamento de Mensagem**
- Se áudio: transcreve para texto
- Se imagem: (futuramente) extrai dados visuais
- Se link: reconhece URL e categoriza como scraping
- Encaminha texto para o orquestrador

**3. Orquestrador**
- Usa IA para identificar a intenção do cliente:
  - Saudação
  - Consulta de veículo
  - Interesse com base em mídia
  - Agendamento
  - Registro ou atualização de lead
- Retorna JSON com `agente_destino` e `mensagem`

**4. Roteador de Agentes**
- Usa switch para redirecionar ao fluxo certo com base em `agente_destino`

**5+. Agentes**
- **BoasVindas:** envia mensagem de saudação personalizada
- **ConsultaVeiculos:** responde com carros filtrados do banco
- **WebScraping:** extrai dados de anúncios enviados e consulta banco
- **Agendamento:** agenda horário com cliente
- **CRM:** cria e atualiza lead no Odoo
- **Fallback:** mensagem genérica ou encaminha para atendimento humano

### Tecnologias Utilizadas
- **N8N** para orquestração modular
- **Zep** para memória conversacional
- **Whisper API** ou OpenAI para transcrição de voz
- **OpenAI Vision** ou modelo customizado para leitura de imagens
- **Playwright / Puppeteer / Cheerio** para scraping
- **CRM Odoo** via API para lead tracking

### Organização dos Flows no N8N

#### Workflows Principais
- `1_Main_EntradaMensagem`
- `2_TratamentoMensagem`
- `3_Orquestrador`
- `4_RoteadorDeAgentes`

#### Subworkflows (Agentes)
- `Agentes/BoasVindas`
- `Agentes/ConsultaVeiculos`
- `Agentes/WebScraping`
- `Agentes/Agendamento`
- `Agentes/CRM`
- `Agentes/Fallback`

### Próximos Passos
- Finalizar os workflows faltantes
- Testar com clientes reais
- Ajustar fluxo de memória contextual
- Implementar fallback com IA generativa

---

## 🔄 FLUXOS OPERACIONAIS COMPLETOS - CASO BIRA VEÍCULOS

### Mapeamento Completo do Processo

A análise dos fluxogramas Miro revela um **mapeamento completo do processo de negócio** de uma concessionária, dividido em 4 quadros principais:

#### **QUADRO 1: Plataforma (Cegonha) - Preparação de Veículos**

**Processo Mapeado:**
- Revisão mecânica
- Pintura veicular
- Martelinho de ouro
- Lavagem
- Polimento
- Entrada no sistema (Autoconfiguração)

**Insight de Negócio:**
A Dobem não apenas automatiza atendimento, mas **mapeia processos completos** do cliente para criar automações end-to-end.

#### **QUADRO 2: Compra - Pré-compra, Avaliação e Precificação**

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

#### **QUADRO 3: Captura de Mídia, Anúncios, Leads e Pré-atendimento**

**Processos:**
- Captura de mídia do carro
- Anúncios
- Captura de Lead
- Pré-atendimento

**Insight de Negócio:**
A Dobem automatiza desde a **captura inicial** até o **pré-atendimento**, criando um funil completo.

#### **QUADRO 4: Venda na Loja - Processo Completo de Venda**

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

---

---

## 🔧 INTEGRAÇÕES E APIs TÉCNICAS

### API Zep (Memória Conversacional)

**1. Criar um "session/user" no Zep:**
```bash
curl -X POST "https://SEU_ZEP_URL/api/v1/sessions" \
  -H "Content-Type: application/json" \
  -d '{
    "id": "cliente-123",
    "metadata": {
      "nome": "Nome do Cliente",
      "origem": "WhatsApp"
    }
  }'
```

**2. Adicionar memória (message history):**
```bash
curl -X POST "https://SEU_ZEP_URL/api/v1/sessions/cliente-123/messages" \
  -H "Content-Type: application/json" \
  -d '{
    "role": "user",
    "content": "Mensagem do usuário"
  }'
```

**3. Buscar memória (histórico):**
```bash
curl -X GET "https://SEU_ZEP_URL/api/v1/sessions/cliente-123/messages?limit=50"
```

**4. Adicionar memória persistente (Zep Memory):**
```bash
curl -X POST "https://SEU_ZEP_URL/api/v1/sessions/cliente-123/memory" \
  -H "Content-Type: application/json" \
  -d '{
    "memory": "Informação persistente sobre o cliente"
  }'
```

### Parar Fluxos n8n

**1. Via interface do n8n (UI):**
- Vá até **Executions** (ou **Execuções**)
- Selecione todas as execuções em andamento (status "running")
- Clique em **"Stop"** (ícone de ⏹️) para cada uma

**2. Via API do n8n:**
```bash
# Listar execuções em andamento:
curl -X GET http://localhost:5678/rest/executions?status=running

# Parar uma execução específica:
curl -X POST http://localhost:5678/rest/executions/:id/stop

# Parar todas as execuções em loop:
for id in $(curl -s http://localhost:5678/rest/executions?status=running | jq -r '.data[].id'); do
  curl -X POST http://localhost:5678/rest/executions/$id/stop
done
```

**3. Via terminal (forçando parada geral):**
```bash
# Docker:
docker restart n8n

# ou se não estiver em Docker:
pm2 restart n8n
# ou
pkill -f n8n
```

### Manter Memória no n8n

**1. Memória temporária (na mesma execução):**
- Use variáveis de workflow (`$json`, `$binary`, etc.)
- Dados persistem apenas durante a execução atual

**2. Memória persistente (entre execuções):**
- **Database (recomendado):** Use PostgreSQL, MySQL ou SQLite
- **Google Sheets / Airtable:** Para dados estruturados
- **Arquivos JSON:** Para armazenamento simples

**3. Memória distribuída (com IA / chatbots):**
- Use **Zep** para memória conversacional
- Use **Redis** para cache rápido
- Use **Vector databases** para busca semântica

**4. Contexto dentro do workflow:**
- Use nós de **Set** para armazenar variáveis
- Use **Function** nodes para manipular dados
- Use **Switch** nodes para roteamento baseado em contexto

### Enviar Mensagem para Typebot

**Exemplo em cURL:**
```bash
curl -X POST "https://typebotapi.bira.dev.biraveiculos.com.br/api/v1/typebots/cm868vsm300058qn4jof7or0b/preview/startChat" \
-H "Content-Type: application/json" \
-d '{"message":"Olá, quero iniciar uma conversa"}'
```

**Exemplo em Python (requests):**
```python
import requests

url = "https://typebotapi.bira.dev.biraveiculos.com.br/api/v1/typebots/cm868vsm300058qn4jof7or0b/preview/startChat"
payload = {
    "message": "Olá, quero iniciar uma conversa"
}
headers = {
    "Content-Type": "application/json"
}

response = requests.post(url, json=payload, headers=headers)
print(response.status_code)
print(response.json())
```

### Receber Áudio no Typebot

**Problema:**
O Typebot não possui suporte nativo para entrada de áudio — ele trabalha com mensagens de texto, botões, formulários, mas não tem um componente para interpretar ou processar áudios diretamente.

**Solução alternativa: Transcrever o áudio antes de enviar ao Typebot**

**Fluxo recomendado:**
1. **Usuário envia áudio via WhatsApp**
2. **Evolution API 2 recebe o áudio** (capturar a URL do arquivo de áudio via webhook)
3. **Usar uma API de transcrição de voz** (Whisper API da OpenAI, ou Google Speech-to-Text) para converter o áudio em texto
4. **O texto transcrito é enviado para o Typebot** como se fosse a mensagem do usuário

**Ferramentas para transcrição:**
- **Whisper API da OpenAI:** Endpoint `https://api.openai.com/v1/audio/transcriptions`
- **Google Cloud Speech-to-Text:** Mais complexo de configurar, mas suporta múltiplos idiomas

**Integração com N8N:**
- Webhook do Evolution recebendo o áudio
- Baixar o áudio (via HTTP Request)
- Passar para o Whisper
- Obter o texto transcrito
- Enviar para o Typebot via Webhook ou API de entrada

---

*Documento consolidado de documentação técnica*
*Última atualização: Dezembro 2025*
