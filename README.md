# 🚨 n8n Server Monitoring & Alerts

Sistema de monitorização de servidores com alertas automáticos, desenvolvido com n8n.

## 📌 Funcionalidades

* Monitorização de uptime via HTTP
* Detecção de falhas (status != 200 ou servidor offline)
* Sistema anti-spam (alertas apenas quando o estado muda)
* Notificações automáticas

## 🧠 Arquitetura

Cron → HTTP Request → Validação → Comparação de estado → Alerta

## ⚙️ Tecnologias

* n8n
* APIs HTTP
* Automação de workflows

## 🚀 Como usar

1. Importa o ficheiro `workflow.json` no n8n
2. Configura as credenciais
3. Define a URL que queres monitorar
4. Ativa o workflow

## 📸 Demonstração

Imagens do projeto na pasta "screenshot".

## 🧠 O que aprendi

* Automação de processos
* Tratamento de erros em workflows
* Integração com APIs externas
* Monitorização de sistemas

## 📈 Melhorias futuras

* Monitorização de múltiplos servidores
* Integração com AWS CloudWatch
* Dashboard de métricas
* Alertas inteligentes com IA
