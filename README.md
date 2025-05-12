# 🌎 E-commerce Internacional - Shopify + Automação via WhatsApp

Este é um projeto de e-commerce desenvolvido para o mercado colombiano, com modelo de **venda por contra entrega (cash on delivery)**. O objetivo é oferecer uma solução rápida, automatizada e centrada na experiência do cliente, desde o primeiro clique até o contato final via WhatsApp.

---

## 🚀 Visão Geral

O projeto foi desenvolvido do zero com foco em performance, usabilidade e automação. A loja foi criada com **Shopify**, integrando um sistema de **captura automática de leads** via **API do WhatsApp (Evolution API)**, com armazenamento e acompanhamento dos pedidos via **Google Sheets**.

---

## ⚙️ Funcionalidades

- 🛒 Loja responsiva criada na Shopify com produtos validados para o mercado colombiano  
- 📩 Captura de leads via formulário na página de produto  
- 🤖 Disparo automático de mensagens no WhatsApp via API (Evolution) usando **n8n**  
- 📊 Armazenamento e controle dos leads em **Google Sheets**  
- 📈 Preparação de estrutura para tráfego pago com **Google Ads e Meta Ads**  
- 🔒 Testes de integração e funcionalidade para garantir estabilidade da operação  

---

## 🧠 Stack Utilizada

### Front-end:
- Shopify (customizações com Liquid, HTML5, CSS3, JavaScript)

### Back-end / Automação:
- Node.js (via [n8n](https://n8n.io/))
- Webhooks personalizados
- API REST (WhatsApp – Evolution API)

### Armazenamento e Dados:
- Google Sheets (planilha integrada com o n8n via credencial segura)

### Outros:
- Postman (para engenharia reversa da API)
- GitHub (versionamento dos scripts de automação)
- Figma (prototipação visual da loja)
- Google Ads / Meta Ads (tráfego e captação de leads)

---

## 🧩 Arquitetura da Solução

```mermaid
graph TD
A[Cliente acessa a loja Shopify] --> B[Formulário preenchido]
B --> C[n8n recebe webhook]
C --> D[API Evolution dispara mensagem no WhatsApp]
C --> E[Lead salvo em Google Sheets]

✅ Resultados Esperados
Redução do tempo de resposta para leads

Centralização dos dados de atendimento

Facilidade no acompanhamento de pedidos

Estrutura pronta para escalar via tráfego pago

🧪 Próximos Passos
Integração com CRM ou banco de dados relacional

Implementação de painel de métricas com Power BI ou Looker Studio

Monitoramento automático de conversão e abandono de pedido

Testes automatizados e validação contínua da API

📌 Observações Técnicas
A documentação oficial da Evolution API é limitada. Para viabilizar a integração, foi realizada engenharia reversa com Postman, inspecionando os headers, payloads e tokens utilizados em chamadas autenticadas, garantindo assim a segurança e a funcionalidade do envio automatizado de mensagens.

👨‍💻 Autor
Luis Gustavo Irigoyen
gustairig.dev@gmail.com
Pelotas, RS – Brasil
Estudante de Análise e Desenvolvimento de Sistemas | Desenvolvedor Full Stack Júnior
