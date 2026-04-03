# ChoiceFeed
The first social media "Buffer" designed to give you back control of your time.

## 🎯 Vision
Oggi i social media sono progettati per massimizzare il Time Spent. FocusFeed ribalta il paradigma: l'obiettivo è massimizzare il _Valore del tempo speso_, categorizzando i contenuti di terze parti (TikTok/Reels) e permettendo all'utente di impostare budget di dopamina rigorosi.

## ⚠️ Il Problema
Gli algoritmi attuali mescolano contenuti educativi con contenuti ad alto rilascio di **dopamina** (brainrot), rendendo impossibile un consumo consapevole. L'utente entra per imparare una ricetta e ne esce dopo due ore di video di prank.

## ✨ La Soluzione: 
- Categorizzazione & FrictionFocusFeed agisce come un filtro intelligente tra le API dei grandi social e l'utente finale:
- Setup Categorie: L'utente sceglie cosa è _"Nutriente"_ (es. Scienza, Politica, Coding) e cosa è "Junk Food" (es. Memes, Prank).
- Time Budgeting: Possibilità di impostare limiti granulari (es. Infinito per Coding, 15 min/giorno per Gossip).
- Smart Interruption: Una volta esaurito il tempo per una categoria, l'app blocca i contenuti di quel tipo, suggerendo di passare a una categoria "produttiva".

## 🛠 Architettura Tecnica Proposta

|Componente|Tecnologia|Ruolo|
|----------|----------|-----|
|Mobile App|Flutter / React Native|Interfaccia utente fluida e cross-platform.|
|Scraper/Aggregator|Node.js + Puppeteer|Recupero link e metadati dai trend.|
|AI Classifier|GPT-4o / Whisper API|Analisi audio/video per assegnazione categoria.|
|Time Engine|Local Storage / Redis|Gestione dei countdown in tempo reale.|

## 🗺 Roadmap di Sviluppo
- Fase 1: Proof of Concept (PoC)Sviluppo di un feed statico con video pre-categorizzati manualmente.Test del sistema di "Time Blocking" interno all'app.
- Fase 2: Integrazione AIImplementazione di un sistema di classificazione automatica tramite trascrizione audio (Speech-to-Text).Testing dei costi delle API per video analizzato.
- Fase 3: Community & SocialPossibilità per gli utenti di votare la categoria di un video (Reinforcement Learning from Human Feedback).

## 🛑 Sfide e Open Issues
- Legalità: Come gestire l'embedding dei video senza violare i TOS di Meta/ByteDance?
- Latenza: L'analisi AI è lenta; serve un sistema di pre-processing dei video di tendenza.
- Monetizzazione: Come rendere sostenibile l'app senza diventare noi stessi degli "spacciatori di attenzione"?
