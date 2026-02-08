# OpenClaw su ZimaOS - Assistente AI Personale

Configurazione completa per un assistente AI personale su ZimaOS con bot Telegram, accesso ai dischi e interfaccia web.

## Cosa fa
- Bot Telegram che risponde in italiano
- Accesso a tutti i dischi del server (SSD, HDD, esterni)
- Legge documenti, PDF, file di testo
- Crea, sposta, rinomina file e cartelle
- Interfaccia web da rete locale
- Completamente gratuito con Groq

## Requisiti
- ZimaOS (o qualsiasi sistema con Docker)
- Account Telegram e bot token (da BotFather)
- Account Groq gratuito (https://console.groq.com)
- Minimo 4GB RAM

## Installazione

### 1. Clona il repository
cd /DATA git clone https://github.com/TelescaAntonio/openclaw-zimaos.git OpenClaw
### 2. Configura le variabili
cp .env.example .env nano .env

### 3. Avvia
docker compose up -d
### 4. Configura il modello
docker compose run --rm openclaw-cli configure --section model
## 5. Parla col bot su Telegram

## Modelli supportati
- Groq (gratis): llama-3.1-8b-instant
- Anthropic (a pagamento): Claude Haiku
- Ollama (locale gratis): richiede piu RAM

## Costi
- Groq: zero euro
- Claude Haiku: circa 1 centesimo per messaggio

## Accesso
- Da casa: http://IP-ZIMAOS:18789
- Da ovunque: Telegram
