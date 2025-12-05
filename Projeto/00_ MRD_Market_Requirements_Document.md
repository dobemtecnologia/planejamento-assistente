# 📊 DORES E INSIGHTS ESTRATÉGICOS - A Base do EVAH

> **Documento de Inteligência de Mercado**
> **Versão:** 2.0 - Consolidada e Verificada
> **Objetivo:** Fundamentar o desenvolvimento do MVP e os argumentos de vendas.

---

## 1. O CONTEXTO: A "FADIGA DE SOFTWARE"

O mercado brasileiro possui **~6 milhões de PMEs**, mas a maioria vive um **colapso operacional silencioso**.
O dono da PME não precisa de "mais uma ferramenta". Ele já tem um CRM, um ERP, um WhatsApp Web e planilhas. O problema é que **nada conversa com nada**.

Chamamos isso de **Fadiga de Software**:
O excesso de ferramentas desconectadas gera mais trabalho do que solução. O EVAH nasce para ser o **"Sistema Operacional"** que conecta essas pontas.

---

## 2. DADOS QUE VALIDAM A DOR (FACT-CHECKING)

Não usamos "achismos". Nossa tese é baseada em dados reais de mercado que comprovam a urgência da automação.

| A Dor do Cliente | O Dado Real (Estatística) | Fonte / Autoridade |
| :--- | :--- | :--- |
| **"Se eu demorar, perco a venda"** | Responder em **5 minutos** aumenta em **21x** a chance de qualificar um lead comparado a 30 minutos. | *Harvard Business Review (HBR)* |
| **"Meu cliente não tem paciência"** | **61%** dos clientes mudam para a concorrência após apenas **uma** experiência ruim de atendimento. | *Zendesk CX Trends* |
| **"Minha equipe só apaga incêndio"** | Cerca de **30%** das atividades em 60% das ocupações poderiam ser automatizadas hoje. | *McKinsey Global Institute* |
| **"Eu não sei o que acontece"** | **79%** dos leads de marketing nunca convertem em vendas por falta de nutrição e dados integrados. | *HubSpot Marketing Stats* |
| **"O futuro é IA"** | Até 2029, agentes de IA resolverão **80%** das solicitações de clientes sem intervenção humana. | *Gartner / IBM* |

---

## 3. AS 3 CAMADAS DE DOR (NÍVEIS DE CONSCIÊNCIA)

Para vender o EVAH, precisamos atacar a dor certa para a pessoa certa.

### 🔴 Camada 1: Dor Operacional (Para o Gerente/Equipe)
*O Caos do Dia a Dia.*
* **Sintoma:** "Tenho que copiar o telefone do WhatsApp e colar no CRM manualmentte."
* **Sintoma:** "Perdi o cliente porque demorei 2 horas para responder o preço."
* **Sintoma:** "Não sei se tem estoque, preciso ligar para o depósito."
* **Solução EVAH:** Automação de tarefas repetitivas (Cadastro automático, Consulta de Estoque).

### 🟡 Camada 2: Dor Estratégica (Para o Dono/CEO)
*A Cegueira dos Dados.*
* **Sintoma:** "Quantos atendimentos viraram venda hoje? Não sei."
* **Sintoma:** "Estou pagando 5 ferramentas e minha equipe continua lenta."
* **Sintoma:** "Meus concorrentes usam IA e eu ainda estou na planilha."
* **Solução EVAH:** Dashboards unificados e redução de custo operacional (fazer mais com menos).

### 🟢 Camada 3: Dor da Experiência (Para o Cliente Final)
*A Frustração do Consumidor.*
* **Sintoma:** "Mandei mensagem sábado e só me responderam segunda-feira."
* **Sintoma:** "Tive que repetir meu CPF três vezes para três atendentes diferentes."
* **Solução EVAH:** Atendimento 24/7 com contexto e memória.

---

## 4. JOBS TO BE DONE (O QUE O CLIENTE REALMENTE QUER)

Não vendemos "software". Vendemos o cumprimento de tarefas (Jobs).

### Job Funcional (A Tarefa)
* "Quero parar de perder tempo cadastrando lead manualmente."
* "Quero responder meu cliente instantaneamente, mesmo de madrugada."
* "Quero saber o preço da Tabela FIPE sem sair do WhatsApp."

### Job Emocional (O Sentimento)
* **Segurança:** "Quero dormir tranquilo sabendo que o robô está atendendo."
* **Controle:** "Quero sentir que minha empresa está na minha mão, não no caos."
* **Orgulho:** "Quero ser visto como uma empresa moderna e tecnológica."

### Job Social (A Percepção)
* "Quero que meu cliente perceba profissionalismo no meu atendimento."
* "Quero mostrar para o mercado que saí da era do papel."

---

## 5. COMO O EVAH RESOLVE (CASES DE USO)

A **Vertical AI** adapta a solução para a dor específica de cada nicho.

#### 🚗 Vertical Automotiva (Case Bira Veículos)
* **Dor:** Cliente pergunta preço no sábado à noite. Vendedor só responde segunda (Lead esfriou).
* **Solução EVAH:** BiraBot atende sábado, consulta FIPE, mostra fotos do carro e agenda visita para segunda de manhã.
* **Ganho:** +40% em agendamentos.

#### 🏠 Vertical Imobiliária
* **Dor:** Corretor perde tempo qualificando "curiosos" que não têm orçamento.
* **Solução EVAH:** Assistente faz triagem (Renda, Localização, Tipo) e só passa para o humano o lead quente.
* **Ganho:** Corretores focados em fechar venda, não em triagem.

#### 🛒 Vertical Varejo/E-commerce
* **Dor:** "Tem esse produto?" (Pergunta repetida 100x por dia).
* **Solução EVAH:** Assistente lê o ERP e responde: "Sim, temos 3 unidades na cor azul."
* **Ganho:** Redução de 60% no volume de suporte humano.

---

## 6. MATRIZ DE PRIORIZAÇÃO DO MVP (DOR → FUNCIONALIDADE)

Esta tabela define o que deve ser construído **AGORA** pelos desenvolvedores. Se a funcionalidade não mata uma dessas dores, ela fica para depois.

| Prioridade | A Dor (Problema Real) | A Funcionalidade (Solução Técnica MVP) |
| :--- | :--- | :--- |
| **CRÍTICA** | "Perco vendas porque demoro a responder." | **Auto-Resposta Imediata:** Integração WhatsApp (Evolution API) + n8n respondendo em < 3s. |
| **CRÍTICA** | "Não sei quem entrou em contato." | **Cadastro Automático:** Criar Lead no Odoo CRM assim que o cliente diz "Oi". |
| **ALTA** | "Agendar reunião é um vai-e-vem de mensagens." | **Agente Calendar:** Integração Google Calendar para cliente escolher horário livre. |
| **ALTA** | "Consultar preço manual é lento." | **Agente de Consulta:** Scraper/Banco de Dados para dar preço (ex: FIPE) na hora. |
| **MÉDIA** | "Cliente odeia falar com robô burro." | **Transbordo Humano:** Botão "Falar com Atendente" que joga para o Chatwoot. |
| **BAIXA** | "Quero ver gráficos bonitos." | **Dashboards:** (Não priorizar no MVP - usar nativo do Odoo). |

---

## 7. CONCLUSÃO PARA O TIME

Este documento prova que a **EVAH** não é uma "ideia legal", é uma **necessidade de mercado**.
As estatísticas mostram que as PMEs estão sangrando dinheiro por ineficiência.
Nossa missão com o MVP é simples: **Estancar esse sangramento** com automação rápida e inteligente.

**Foco do MVP:** Velocidade de Resposta + Execução de Tarefa (Agendar/Consultar). Todo o resto é ruído.