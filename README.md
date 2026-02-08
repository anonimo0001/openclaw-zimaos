# OpenClaw ZimaOS - Assistente AI Locale con Telegram

Un assistente AI personale che gira sul tuo server domestico, senza costi API, controllabile da Telegram ovunque.

## Cosa fa

- Gira sul TUO hardware, a casa tua
- Costa zero euro al mese
- Si controlla da Telegram ovunque
- Ha accesso ai tuoi file e dischi esterni
- Legge PDF, manuali, documenti
- Crea, sposta, organizza file e cartelle

## Requisiti

- ZimaOS o qualsiasi PC con Docker
- Minimo 8GB RAM
- 10GB spazio disco per il modello AI
- Un bot Telegram (gratuito da BotFather)

## Installazione

1. Installa Ollama: docker run -d --name ollama --restart unless-stopped -p 11434:11434 -v ollama_data:/root/.ollama ollama/ollama
2. Scarica modello: docker exec ollama ollama pull llama3.1:8b
3. Clona repo: git clone https://github.com/anonimo0001/openclaw-zimaos.git
4. Configura: cp .env.example .env e modifica
5. Avvia: docker compose up -d
6. Configura modello: docker compose run --rm openclaw-cli configure --section model

## Modelli supportati

- Ollama locale (gratis): llama3.1:8b
- Groq cloud (gratis): llama-3.1-8b-instant
- Claude Haiku (1 cent/messaggio)

## Sicurezza

Il modello AI gira localmente. I tuoi dati non escono di casa.

## Autore

Antonio Telesca
