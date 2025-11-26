# 💼 NEGÓCIO - Análise Estratégica dos Fluxogramas Miro

> **Fonte:** Análise profunda de 41 prints do quadro Miro  
> **Data de análise:** 2025  
> **Objetivo:** Compreender o modelo de negócio, fluxos operacionais e estratégias da Dobem Tecnologia

---

## 🎯 1. MODELO DE NEGÓCIO IDENTIFICADO: VERTICAL AI

### 1.1 Definição Estratégica

A Dobem Tecnologia adota um **modelo de negócio Vertical AI**, que representa uma mudança fundamental de paradigma:

**Não é SaaS tradicional:**
- ❌ Não vende software como serviço genérico
- ✅ Vende **fluxos de otimização de operação** especializados

**Diferencial:**
- Especialização em nichos específicos de mercado
- Uso de Inteligência Artificial para automatizar processos únicos de cada setor
- Adaptação a qualquer negócio, mas com profundidade vertical

### 1.2 Aplicação Prática: Caso Bira Veículos

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

### 1.3 Estratégia de Venda

**Abordagem:**
- Criar várias soluções integradas utilizando IA
- Esse conjunto forma uma solução em um nicho específico de mercado
- As possibilidades são infinitas

**Valor Proposto:**
"Fluxos de otimização de operação" ao invés de "software"

---

## 🏗️ 2. ARQUITETURA DE VALOR: ECOSSISTEMA EVAH

### 2.1 Visão Geral do Ecossistema

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

### 2.2 Arquitetura Modular de Agentes

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

---

## 🔄 3. FLUXOS OPERACIONAIS COMPLETOS - ANÁLISE DO CASO BIRA VEÍCULOS

### 3.1 Mapeamento Completo do Processo

A análise dos prints revela um **mapeamento completo do processo de negócio** de uma concessionária, dividido em 4 quadros principais:

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

---

## 💡 4. CONCLUSÕES SOBRE O MODELO DE NEGÓCIO

### 4.1 Diferenciação Estratégica

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

### 4.2 Proposta de Valor Única

**Para o Cliente:**
- "Não vendemos software, vendemos otimização de operação"
- "Automatizamos processos que só humanos faziam"
- "Criamos agentes especializados para seu negócio"

**Diferencial:**
- Entendimento profundo do negócio do cliente
- Mapeamento completo de processos
- Automação de tarefas que pareciam impossíveis de automatizar

### 4.3 Modelo de Receita

**Identificado nos Prints:**

**Kits de Produtos:**
- KIT SETUP STARTUP: R$ 3.000,00
- KIT VENDA ATENDIMENTO: R$ 3.000,00
- KIT SETUP PET: R$ 3.000,00

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

## 🎯 5. DORES DO CLIENTE MAPEADAS

### 5.1 Problemas Operacionais Identificados

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

### 5.2 Oportunidade de Mercado

**Conclusão:**
As empresas não precisam apenas de "um chatbot" ou "um CRM". Elas precisam de:
- **Visibilidade** sobre o que acontece no atendimento
- **Histórico** de todas as interações
- **Automação** de processos repetitivos
- **Métricas** para tomar decisões
- **Controle** sobre leads e oportunidades

**A Dobem resolve isso com um ecossistema integrado.**

---

## 🏭 6. INFRAESTRUTURA E HOSPEDAGEM - MODELOS DE NEGÓCIO

### 6.1 Dois Modelos Identificados

#### **Modelo 1: Servidor Dedicado (Onpremisse)**
- Cada empresa tem seu próprio servidor
- Isolamento total
- Maior controle e segurança
- Custo mais alto

#### **Modelo 2: Servidor Compartilhado (SaaS)**
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

### 6.2 Stack Tecnológico Identificado

**Infraestrutura:**
- AWS EC2 (Large)
- Docker Swarm
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

---

## 🤖 7. FLUXOS DE PROCESSAMENTO - ANÁLISE TÉCNICA

### 7.1 Fluxo de Processamento de Mensagens

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

### 7.2 Fluxo de Captura e Qualificação de Lead

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

### 7.3 Fluxo de Agendamento

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

---

## 💰 8. ANÁLISE DE PREÇOS E ESTRUTURA COMERCIAL

### 8.1 Kits de Produtos

**Estratégia Identificada:**
- **KIT SETUP STARTUP:** R$ 3.000,00
- **KIT VENDA ATENDIMENTO:** R$ 3.000,00
- **KIT SETUP PET:** R$ 3.000,00

**Análise:**
- **Preço de entrada:** R$ 3.000 é acessível para PMEs
- **Pacotes temáticos:** Por setor/necessidade
- **Valor percebido:** "Kit completo" soa melhor que "serviços avulsos"

### 8.2 Estrutura de Preços Modular

**Componentes Identificados:**
- OpenAI: Custo variável (uso)
- Zepli: Custo variável
- Licença Odoo: Custo variável
- Número de workflows: Custo variável
- Número de assistentes IA: Custo variável

**Análise:**
- **Modelo híbrido:** Setup fixo + uso variável
- **Escalabilidade:** Cliente paga conforme cresce
- **Transparência:** Custo por componente
- **Flexibilidade:** Cliente escolhe o que precisa

### 8.3 Cálculo Dinâmico de Planos

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

## 🎯 9. CONCLUSÕES ESTRATÉGICAS

### 9.1 Modelo de Negócio: Vertical AI

**Características:**
1. **Especialização por setor:** Não é genérico, é específico
2. **Profundidade:** Entende processos completos do cliente
3. **Automação inteligente:** IA para tarefas que pareciam impossíveis
4. **Ecossistema integrado:** Não vende produtos, vende soluções completas

### 9.2 Vantagem Competitiva

**Diferenciais Identificados:**

1. **Mapeamento Completo de Processos:**
   - Não apenas automatiza atendimento
   - Mapeia e automatiza processos end-to-end
   - Exemplo: Quadro completo de venda de veículos

2. **Agentes Especializados:**
   - Cada agente faz uma coisa muito bem
   - Orquestração inteligente
   - Personalização profunda por cliente

3. **Flexibilidade de Infraestrutura:**
   - Onpremisse ou SaaS
   - Cliente escolhe conforme necessidade
   - Permite migração

4. **Modelo de Preço Justo:**
   - Setup acessível (R$ 3.000)
   - Custos variáveis transparentes
   - Escala conforme uso

### 9.3 Oportunidades de Mercado

**Setores Identificados nos Prints:**
1. **Concessionárias de Veículos** (Bira Veículos - caso real)
2. **Startups** (KIT SETUP STARTUP)
3. **Pet Shops/Veterinárias** (KIT SETUP PET)
4. **Vendas e Atendimento** (KIT VENDA ATENDIMENTO)

**Potencial:**
- Cada setor tem processos únicos
- Cada processo pode ser automatizado
- As possibilidades são infinitas

### 9.4 Riscos e Desafios Identificados

**1. Complexidade de Implementação:**
- Mapear processos completos é trabalhoso
- Requer entendimento profundo do negócio do cliente
- **Mitigação:** Kits pré-configurados por setor

**2. Dependência de APIs Externas:**
- OpenAI, Google, etc. têm custos variáveis
- Mudanças em APIs podem impactar
- **Mitigação:** Diversificação de provedores

**3. Escalabilidade do Modelo:**
- Cada cliente precisa de personalização
- Pode ser difícil escalar sem perder qualidade
- **Mitigação:** Agentes reutilizáveis + personalização pontual

### 9.5 Recomendações Estratégicas

**1. Focar em Setores Específicos:**
- Criar "soluções prontas" para setores (como os kits)
- Acelerar time-to-market
- Reduzir custo de implementação

**2. Desenvolver Biblioteca de Agentes:**
- Agentes reutilizáveis por função
- Personalização apenas onde necessário
- Escalabilidade mantendo qualidade

**3. Documentar Processos:**
- Criar templates de mapeamento de processos
- Facilitar onboarding de novos clientes
- Acelerar implementação

**4. Métricas e ROI:**
- Medir impacto real das automações
- Demonstrar ROI claro para clientes
- Cases de sucesso com números

**5. Parcerias Estratégicas:**
- Parcerias com empresas de setores específicos
- Co-marketing
- Referências qualificadas

---

## 📊 10. ANÁLISE DE VALOR ENTREGUE

### 10.1 Valor para o Cliente

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

### 10.2 Diferenciação vs. Concorrentes

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

## 🚀 11. PRÓXIMOS PASSOS ESTRATÉGICOS

### 11.1 Desenvolvimento de Produto

**Prioridades:**
1. Finalizar MVP do EVAH
2. Criar mais kits por setor (além dos 3 atuais)
3. Desenvolver biblioteca de agentes reutilizáveis
4. Melhorar documentação de processos

### 11.2 Go-to-Market

**Estratégias:**
1. Focar em setores específicos inicialmente
2. Criar cases de sucesso (Bira Veículos como primeiro)
3. Desenvolver materiais de venda por setor
4. Parcerias estratégicas

### 11.3 Operações

**Melhorias:**
1. Padronizar processo de mapeamento de processos
2. Criar templates de implementação
3. Desenvolver ferramentas de cálculo de ROI
4. Sistema de métricas e acompanhamento

---

## 📝 12. OBSERVAÇÕES FINAIS

### 12.1 Forças do Modelo

1. **Diferenciação clara:** Vertical AI é único no mercado
2. **Valor mensurável:** ROI tangível para clientes
3. **Escalabilidade técnica:** Arquitetura moderna e flexível
4. **Flexibilidade comercial:** Múltiplos modelos de preço

### 12.2 Desafios

1. **Educação de mercado:** Cliente precisa entender o conceito de Vertical AI
2. **Complexidade de venda:** Requer entendimento profundo do negócio do cliente
3. **Tempo de implementação:** Mapear processos leva tempo
4. **Dependência de expertise:** Requer equipe técnica especializada

### 12.3 Oportunidades

1. **Mercado em crescimento:** IA e automação em alta
2. **Dores reais:** Clientes têm problemas que a Dobem resolve
3. **Diferenciação:** Poucos concorrentes com modelo similar
4. **Escalabilidade:** Uma vez mapeado, pode replicar por setor

---

**Última atualização:** 2025  
**Fonte:** Análise estratégica de 41 prints do quadro Miro  
**Análise realizada por:** Interpretação de fluxogramas e padrões de negócio
