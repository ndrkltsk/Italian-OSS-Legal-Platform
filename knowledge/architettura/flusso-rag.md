---
type: Processo
title: Flusso di una domanda (RAG)
description: Sequenza dal quesito dell'utente alla risposta con citazioni verificabili.
tags: [rag, retrieval, citazioni]
timestamp: 2026-06-18T00:00:00Z
---

# Flusso di una domanda (RAG)

1. L'utente pone una domanda in linguaggio naturale.
2. Il [backend](/architettura/backend-api.md) recupera i [Chunk](/modello-dati/chunk.md) più rilevanti dall'[indice](/architettura/indice-normativo.md) ([ricerca semantica](/glossario/ricerca-semantica.md) + filtri).
3. Costruisce un contesto con i testi normativi e i relativi metadati di citazione.
4. L'[LLM](/architettura/provider-llm.md) genera la risposta **citando** articolo, comma e fonte ([ELI](/glossario/eli.md)).
5. Il [frontend](/architettura/frontend.md) mostra la risposta con i link verificabili alle fonti.

Vedi [RAG](/glossario/rag.md) e [citazione verificabile](/glossario/citazione-verificabile.md).
