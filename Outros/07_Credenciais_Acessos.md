# 🔐 CREDENCIAIS E ACESSOS

## 📋 Índice
- [Credenciais de Sistema](#credenciais-de-sistema)
- [Acessos à Infraestrutura](#acessos-à-infraestrutura)
- [APIs e Integrações](#apis-e-integrações)
- [Segurança](#segurança)

---

## 🔑 Credenciais de Sistema

### Google

- **Link:** [Google](https://www.google.com.br)
- **Login:** `marketing.dobemtecnologia@gmail.com`
- **Senha:** `d0b3mT3ch`

**Observação:** Esta é uma credencial de acesso ao Google. Mantenha em local seguro e considere usar um gerenciador de senhas.

## 🖥️ Acessos à Infraestrutura

### AWS (Amazon Web Services)

**Serviços Utilizados:**
- **EC2** - Instâncias de servidor
- **ECS (Elastic Container Service)** - Orquestração de containers
  - Cluster: `dobemtech-cluster`
  - Task Family: `dobemtech-task`
  - Log Group: `/ecs/dobemtech`
- **RDS** - Banco de dados PostgreSQL
- **S3** - Armazenamento de arquivos
- **Lambdas** - Funções serverless

**Domínios e URLs:**
- **Domínio Principal:** dobemtecnologia.com
- **Domínios Alternativos:** dobemtech.com, www.dobemtech.com
- **Subdomínios Configurados:**
  - odoo.dobemtech.com
  - www.dobemtecnologia.com
  - erp.dobemtecnologia.com
  - n8n.aws.biraveiculos.com.br
  - webhook.aws.biraveiculos.com.br
  - evo-api.aws.biraveiculos.com.br

### Docker Swarm

**Stacks em Execução:**
- **Traefik** - Proxy reverso e load balancer
- **Portainer** - Gerenciamento de containers
- **n8n** - Automação e orquestração
- **Odoo** - ERP
- **Chatwoot** - Atendimento omnichannel
- **Evolution API** - Integração WhatsApp

### Banco de Dados

**PostgreSQL (RDS):**
- **Host exemplo:** db-postgres.cboyyg6aixgi.us-east-1.rds.amazonaws.com
- **Porta:** 5432
- **Database n8n:** n8n
- **Database Odoo:** odoo

**Observação:** Credenciais específicas devem ser armazenadas em cofre de senhas seguro.

## 🔗 APIs e Integrações

### OpenAI (ChatGPT)

**Uso:**
- API para processamento de linguagem natural
- Transcrição de áudio (Whisper API)
- Análise de imagens
- Geração de respostas contextuais

**Custos:**
- Input: Variável conforme modelo
- Output: Variável conforme modelo
- Transcrição de áudio: R$ 0,02 por mensagem
- Análise de imagens: R$ 0,02 por imagem

### Google APIs

**Google Calendar API:**
- OAuth 2.0 Client ID necessário
- Permissões para criar, consultar e gerenciar eventos

**Google Drive API:**
- Upload, download e organização de arquivos
- Controle de permissões

**Google Cloud Speech-to-Text:**
- Alternativa ao Whisper para transcrição de áudio

### Evolution API

**Uso:**
- Integração com WhatsApp
- Webhooks para recebimento de mensagens
- Envio de mensagens e mídias

**Configuração:**
- Host: evo-api.aws.biraveiculos.com.br (exemplo)
- Webhook URL: https://webhook.aws.biraveiculos.com.br/webhook/...

### Meta APIs

**WhatsApp Business API (Oficial):**
- Integração via API oficial do Meta
- Conformidade com políticas do WhatsApp
- Custos: R$ 0,03 por mensagem

**Instagram API:**
- Integração com Direct Messages
- Custos: R$ 0,03 por mensagem

**Facebook Messenger API:**
- Integração com Messenger
- Custos: R$ 0,03 por mensagem

### Outras APIs

**FIPE API:**
- Consulta de valores de veículos
- Integração para cotações automotivas

**Gateways de Pagamento:**
- PagSeguro (exemplo)
- Custos: R$ 3,50 por transação (exemplo)

## 🛡️ Segurança

### Boas Práticas

**Armazenamento de Credenciais:**
- Armazenar todos os logins e senhas em um cofre de senhas adequado
- Não commitar credenciais em repositórios de código
- Usar variáveis de ambiente para credenciais sensíveis
- Rotacionar senhas periodicamente

**Centralização de Emails:**
- Centralizar emails de acordo com os Alias em todas as aplicações
- Usar emails corporativos para serviços importantes

**Monitoramento:**
- Uptime Kuma para monitoramento de APIs, sites, etc.
- Monitoramento contínuo de custos e desempenho AWS
- Alertas configuráveis para falhas e inconsistências

**SSL/TLS:**
- Certificados Let's Encrypt via Traefik
- HTTPS obrigatório para todos os serviços
- Validação de certificados SSL

**Autenticação:**
- APIs com autenticação e autorização
- Tokens de acesso para serviços externos
- OAuth 2.0 para integrações Google

**Criptografia:**
- Dados criptografados em trânsito e em repouso
- Chaves de criptografia para n8n e outros serviços
- Conformidade com LGPD

### Configurações Importantes

**n8n:**
- `N8N_ENCRYPTION_KEY`: Chave de criptografia (manter segura)
- `N8N_ENFORCE_SETTINGS_FILE_PERMISSIONS`: true
- `N8N_COMMUNITY_PACKAGES_ENABLED`: true (se necessário)

**Docker Swarm:**
- Configuração de networks isoladas
- Security groups configurados
- Volumes persistentes para dados importantes

**AWS:**
- Security groups com regras mínimas necessárias
- IAM roles com permissões mínimas
- Backup automático de bancos de dados

---

*Documento consolidado de credenciais e acessos*
*Última atualização: Dezembro 2025*

**⚠️ IMPORTANTE:** Este documento contém informações sensíveis. Mantenha em local seguro e com acesso restrito.
