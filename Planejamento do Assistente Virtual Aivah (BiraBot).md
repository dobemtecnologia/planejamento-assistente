[https://chatgpt.com/c/6882a96c-2130-8007-a12f-539bda118e61](https://chatgpt.com/c/6882a96c-2130-8007-a12f-539bda118e61)

\# Planejamento do Assistente Virtual Aiva (BiraBot) para a Bira Veículos

\#\# 📌 Visão Geral  
Aiva (nome técnico), apresentado aos clientes como \*\*BiraBot\*\*, é um assistente virtual desenvolvido pela Bain Tecnologia para realizar \*\*atendimento automatizado em empresas de venda de veículos\*\*, com foco em:

\- Atendimento inicial com boas-vindas  
\- Entendimento do interesse do cliente  
\- Consulta de veículos disponíveis  
\- Registro e atualização de leads no CRM (Odoo)  
\- Agendamento de visitas  
\- Interpretação de mídia (áudio, imagem, link)  
\- Consulta baseada em links (web scraping)

\---

\#\# 🎯 Objetivos do Assistente

\#\#\# ✅ Comunicação Inicial  
\- Detectar e responder a saudações como "bom dia", "boa tarde", "olá", etc.  
\- Apresentar-se como BiraBot e explicar sua função

\#\#\# ✅ Coleta de Interesse do Cliente  
\- Identificar tipo de veículo desejado  
\- Extrair informações como:  
  \- Marca / modelo  
  \- Tipo (SUV, hatch, sedan...)  
  \- Ano mínimo e máximo  
  \- Faixa de preço

\#\#\# ✅ Consulta de Veículos  
\- Integrar com agente que consulta banco de dados  
\- Apresentar resultados baseados nos filtros coletados

\#\#\# ✅ Registro e Qualificação de Lead  
\- Integrar com CRM Odoo para:  
  \- Criar lead no início do atendimento  
  \- Atualizar lead à medida que mais dados são fornecidos

\#\#\# ✅ Agendamento de Visita  
\- Perguntar disponibilidade do cliente  
\- Registrar data e hora sugerida  
\- (Futuramente: integrar com agenda de vendedores)

\#\#\# ✅ Interpretação Multimídia  
\- \*\*Áudio\*\*:  
  \- Transcrever voz em texto  
  \- Passar texto para o orquestrador  
\- \*\*Imagem\*\*:  
  \- Extrair dados visuais (modelo, tipo, cor)  
  \- Consultar no banco veículos semelhantes  
\- \*\*Link (Web Scraping)\*\*:  
  \- Extrair dados de anúncios (OLX, Webmotors, etc.)  
  \- Realizar consulta no banco com base nesses dados

\#\#\# ✅ Memória e Contexto  
\- Usar memória (ex: Zep) para manter o histórico do cliente  
\- Ex: "Quero um carro de 2022" \+ depois "quero que seja SUV" → entender que busca é SUV de 2022

\---

\#\# 🧠 Arquitetura Modular no N8N

\#\#\# 🔁 Fluxo Geral:  
1\. \*\*1\_Main\_EntradaMensagem\*\* – Entrada de texto, áudio ou imagem  
2\. \*\*2\_TratamentoMensagem\*\* – Converte áudio, texto, imagem em texto limpo  
3\. \*\*3\_Orquestrador\*\* – Detecta a intenção do cliente  
4\. \*\*4\_RoteadorDeAgentes\*\* – Direciona para o agente correto com base na intenção  
5\. \*\*Agentes Específicos\*\*:  
   \- 5\_AgenteBoasVindas  
   \- 6\_AgenteConsultaVeiculos  
   \- 7\_AgenteWebScraping  
   \- 8\_AgenteAgendamento  
   \- 9\_AgenteCRM  
   \- 10\_AgenteDesconhecido (Fallback)

\#\#\# 🧩 Módulos e Funções

\#\#\#\# 1\. Entrada  
\- Recebe mensagem  
\- Redireciona para tratamento

\#\#\#\# 2\. Tratamento de Mensagem  
\- Se áudio: transcreve para texto  
\- Se imagem: (futuramente) extrai dados visuais  
\- Se link: reconhece URL e categoriza como scraping  
\- Encaminha texto para o orquestrador

\#\#\#\# 3\. Orquestrador  
\- Usa IA para identificar a intenção do cliente:  
  \- Saudação  
  \- Consulta de veículo  
  \- Interesse com base em mídia  
  \- Agendamento  
  \- Registro ou atualização de lead  
\- Retorna JSON com \`agente\_destino\` e \`mensagem\`

\#\#\#\# 4\. Roteador de Agentes  
\- Usa switch para redirecionar ao fluxo certo com base em \`agente\_destino\`

\#\#\#\# 5+. Agentes  
\- \*\*BoasVindas\*\*: envia mensagem de saudação personalizada  
\- \*\*ConsultaVeiculos\*\*: responde com carros filtrados do banco  
\- \*\*WebScraping\*\*: extrai dados de anúncios enviados e consulta banco  
\- \*\*Agendamento\*\*: agenda horário com cliente  
\- \*\*CRM\*\*: cria e atualiza lead no Odoo  
\- \*\*Fallback\*\*: mensagem genérica ou encaminha para atendimento humano

\---

\#\# 🛠️ Tecnologias Utilizadas  
\- \*\*N8N\*\* para orquestração modular  
\- \*\*Zep\*\* para memória conversacional  
\- \*\*Whisper API\*\* ou OpenAI para transcrição de voz  
\- \*\*OpenAI Vision ou modelo customizado\*\* para leitura de imagens  
\- \*\*Playwright / Puppeteer / Cheerio\*\* para scraping  
\- \*\*CRM Odoo\*\* via API para lead tracking

\---

\#\# 📦 Organização dos Flows no N8N

\#\#\# Workflows Principais  
\- \`1\_Main\_EntradaMensagem\`  
\- \`2\_TratamentoMensagem\`  
\- \`3\_Orquestrador\`  
\- \`4\_RoteadorDeAgentes\`

\#\#\# Subworkflows (Agentes)  
\- \`Agentes/BoasVindas\`  
\- \`Agentes/ConsultaVeiculos\`  
\- \`Agentes/WebScraping\`  
\- \`Agentes/Agendamento\`  
\- \`Agentes/CRM\`  
\- \`Agentes/Fallback\`

\---

\#\# ✅ Próximos Passos  
\- Finalizar os workflows faltantes  
\- Testar com clientes reais  
\- Ajustar fluxo de memória contextual  
\- Implementar fallback com IA generativa

\---

Se precisar de ajustes, novos agentes ou exportações em JSON, posso continuar gerando conforme seu progresso. ✨

