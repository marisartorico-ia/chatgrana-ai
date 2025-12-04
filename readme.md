# 💰 ChatGrana.ai

> Seu assistente financeiro inteligente direto no WhatsApp

## 📋 Sobre o Projeto

O **ChatGrana.ai** é uma solução fintech inovadora que utiliza Inteligência Artificial para ajudar consumidores brasileiros a controlarem suas finanças pessoais de forma simples e intuitiva, através do WhatsApp.

### Problema

Muitas pessoas têm dificuldade em:
- Controlar gastos diários
- Entender para onde vai seu dinheiro
- Manter disciplina financeira
- Usar aplicativos complexos de finanças

### Solução

Uma IA conversacional no WhatsApp que:
- Registra gastos de forma natural (texto, áudio ou foto)
- Gera insights personalizados automaticamente
- Envia alertas proativos sobre orçamento
- Cria relatórios visuais simplificados

## 🎯 Funcionalidades Principais

### 1. Registro Inteligente de Gastos
- **Por texto**: "Gastei R$ 45 no almoço"
- **Por áudio**: Mensagens de voz processadas automaticamente
- **Por foto**: OCR de notas fiscais para extração automática de dados

### 2. Análise com IA
- Categorização automática de despesas
- Identificação de padrões de consumo
- Comparações temporais (semana/mês)
- Previsões de gastos futuros

### 3. Insights Personalizados
- "Você gastou 30% a mais em delivery este mês"
- "Seus gastos com transporte diminuíram"
- Sugestões de economia baseadas em comportamento

### 4. Alertas Proativos
- Notificações de limite de orçamento
- Lembretes de contas a pagar
- Avisos de gastos incomuns

### 5. Relatórios Visuais
- Gráficos de pizza por categoria
- Evolução temporal de gastos
- Resumos mensais automáticos
- Exportação de dados

## 🛠️ Tecnologias Utilizadas

### Frontend (Landing Page)
- **HTML5**: Estrutura semântica
- **CSS3**: Estilização e animações
- **Bootstrap 5**: Framework responsivo

### Backend (Arquitetura Proposta)
- **Python 3.x**: Linguagem principal
- **Flask/FastAPI**: Framework web
- **WhatsApp Business API**: Integração com WhatsApp
- **OpenAI GPT**: Processamento de linguagem natural
- **Tesseract OCR**: Leitura de notas fiscais
- **Pandas**: Análise de dados
- **Matplotlib/Plotly**: Geração de gráficos

### Banco de Dados
- **PostgreSQL**: Armazenamento de dados estruturados
- **Redis**: Cache e sessões

### Infraestrutura
- **Docker**: Containerização
- **GitHub Actions**: CI/CD
- **AWS/Heroku**: Hospedagem

## 🏗️ Arquitetura do Sistema

```
┌─────────────┐
│  WhatsApp   │
│   (User)    │
└──────┬──────┘
       │
       ▼
┌─────────────────────┐
│  WhatsApp Business  │
│       API           │
└──────┬──────────────┘
       │
       ▼
┌─────────────────────┐
│   API Gateway       │
│   (Flask/FastAPI)   │
└──────┬──────────────┘
       │
       ├──────────────────┐
       ▼                  ▼
┌─────────────┐    ┌─────────────┐
│  IA Engine  │    │  Database   │
│  (GPT + OCR)│    │ (PostgreSQL)│
└──────┬──────┘    └─────────────┘
       │
       ▼
┌─────────────────────┐
│  Analytics Engine   │
│  (Pandas + Plotly)  │
└─────────────────────┘
```

## 🚀 Como Usar

### Para Usuários

1. Adicione o número do ChatGrana.ai no WhatsApp
2. Envie uma mensagem para iniciar
3. Comece a registrar seus gastos naturalmente
4. Receba insights e relatórios automaticamente

### Para Desenvolvedores

```bash
# Clone o repositório
git clone https://github.com/marisartorico-ia/chatgrana-ai.git

# Entre no diretório
cd chatgrana-ai

# Instale as dependências
pip install -r requirements.txt

# Configure as variáveis de ambiente
cp .env.example .env

# Execute o servidor
python app.py
```

## 📁 Estrutura do Projeto

```
chatgrana-ai/
├── index.html              # Landing page
├── README.md              # Este arquivo
├── src/
│   ├── app.py            # Aplicação principal
│   ├── whatsapp/         # Integração WhatsApp
│   ├── ai/               # Módulos de IA
│   ├── database/         # Modelos e conexões
│   └── analytics/        # Geração de insights
├── static/               # Arquivos estáticos
├── docs/                 # Documentação adicional
└── tests/                # Testes automatizados
```

## 🔐 Segurança e Privacidade

- Criptografia end-to-end nas comunicações
- Dados armazenados com criptografia AES-256
- Conformidade com LGPD (Lei Geral de Proteção de Dados)
- Autenticação de dois fatores
- Logs de auditoria completos

## 📊 Diferenciais Competitivos

| Recurso | ChatGrana.ai | Apps Tradicionais |
|---------|--------------|-------------------|
| Interface | WhatsApp | App dedicado |
| Curva de aprendizado | Zero | Alta |
| Registro de gastos | Texto/Áudio/Foto | Manual |
| IA integrada | ✅ | Limitada |
| Disponibilidade | 24/7 | Requer abertura |
| Custo inicial | Gratuito | Freemium |

## 🎓 Contexto Acadêmico

Este projeto foi desenvolvido como parte do **Checkpoint 9 - Muito estilo sem sofrimento** da FIAP, que exige:

- Criação de página no GitHub
- Utilização de HTML, CSS e Bootstrap
- Desenvolvimento de ideia de fintech inovadora
- Aplicação do GitHub Flow
- Repositório público

## 👥 Equipe

- **Desenvolvedor**: Maria Vitória Rodrigues
- **RM**: rm566938

---

**ChatGrana.ai** - Transformando conversas em controle financeiro 💰📱