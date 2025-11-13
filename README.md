# Documentação Técnica do Projeto n8n - Automação Comercial com IA e ElevenLabs

## Visão Geral
Este projeto automatiza o processo comercial de prospecção usando um agente de SDR alimentado por Inteligência Artificial, integrado diretamente com a tecnologia de voz da ElevenLabs. A automação combina IA para geração de conteúdo, multicanalidade de comunicação e insights inteligentes para potencializar a eficiência das vendas outbound.

---

## Componentes Principais do Workflow

### 1. Captação e Validação de Leads
- Extração e normalização de dados de contatos (e-mail, telefone, nome).
- Uso de expressões regulares para validação precisa de e-mails.
- Controle de status dos contatos em banco Redis, evitando contatos duplicados.

### 2. Geração e Personalização com IA
- Utilização de modelos avançados de linguagem (OpenAI GPT via Langchain) para criação automatizada de textos.
- Produção de textos comerciais persuasivos para e-mails de prospecção.
- Pesquisa contextual feita pela IA para identificar pontos de interesse na empresa alvo.
- **Contexto integrado com ElevenLabs para síntese de voz natural e chamadas por voz automatizadas**, ampliando a comunicação humana com tecnologia de ponta.

### 3. Comunicação Multicanal Automatizada
- Envio de e-mails personalizados via Gmail API.
- Follow-ups por WhatsApp integrados via HTTP Requests a plataformas externas.
- Chamadas telefônicas automatizadas com voz gerada pela IA da ElevenLabs, proporcionando contato mais humano e personalizado.
- Registros e atualizações constantes em Google Sheets para acompanhamento detalhado do fluxo comercial.

### 4. Monitoramento e Gestão de Respostas
- Detecção automática de respostas por e-mail para segmentar próximos passos.
- Lógica condicional para planejar ações de follow-up ou encerramento do contato.
- Sincronização com Redis para controle robusto do ciclo do lead.

### 5. Planejamento e Agendamento de Atividades
- Gatilhos temporais para realizar envios e ligações em horários estratégicos.
- Criação de lembretes e eventos de calendarização vinculados ao progresso do fluxo.

---

## Tecnologias e Integrações

| Tecnologia           | Função                                                |
|---------------------|------------------------------------------------------|
| n8n                 | Orquestração do fluxo de automação                    |
| OpenAI GPT via Langchain | Geração dinâmica de texto e pesquisa contextual    |
| ElevenLabs IA de Voz | Síntese de voz natural e chamadas telefônicas         |
| Redis               | Banco de dados para controle de status e flags        |
| Gmail API           | Envio e monitoramento de e-mails                       |
| HTTP Requests       | Integração com APIs externas (WhatsApp, telefonia)    |
| Google Sheets       | CRM leve para registro e análise das interações       |

---

## Benefícios Comerciais

- **Personalização inteligente e rápida:** A IA entende a empresa-alvo e cria mensagens com alto grau de aderência.
- **Multicanalidade com voz natural:** Diferenciação competitiva com chamadas automatizadas de alta qualidade usando ElevenLabs.
- **Escalabilidade eficiente:** Automação 24/7 com controle rigoroso para evitar spam e respeitar jornada do cliente.
- **Dados em tempo real:** Atualização constante e rastreamento no CRM para decisões rápidas e estratégias ajustáveis.

---

## Considerações para o GitHub

- Documentação feita em Markdown limpa, clara e objetiva para fácil visualização.
- Atenção especial ao destaque da integração diferenciada com IA de voz ElevenLabs para efeito comercial.
- Conteúdo voltado para desenvolvedores e equipes comerciais que irão gerir e otimizar o fluxo.
- Modularidade para facilitar manutenção, customização e escalabilidade futuras.

---

> Esta documentação está preparada para ser usada diretamente em seu repositório GitHub, equilibrando clareza técnica e foco comercial com ênfase na poderosa integração de IA para automação comercial.

