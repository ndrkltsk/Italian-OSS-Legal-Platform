---
type: Processo
title: Pipeline di trasformazione
description: Dal download AKN di Normattiva fino all'indice vettoriale e al grafo dei riferimenti, preservando i metadati di citazione.
tags: [pipeline, ingest, chunking, embedding]
timestamp: 2026-06-18T00:00:00Z
---

# Pipeline di trasformazione

```
Normattiva (API)
   │  download AKN + metadati ELI
   ▼
Parsing AKN  ──►  estrazione struttura (Work/Expression/Unità)
   │
   ▼
Normalizzazione testo  (preservando i riferimenti)
   │
   ▼
Chunking per unità  (articolo/comma, con metadati di citazione)
   │
   ▼
Embedding  ──►  indice vettoriale
   │
   ▼
Estrazione riferimenti  ──►  grafo delle norme
```

**Principio chiave**: ogni [Chunk](/modello-dati/chunk.md) porta con sé i metadati necessari a costruire una **[citazione verificabile](/glossario/citazione-verificabile.md)** ([ELI](/glossario/eli.md) + articolo + comma + data di vigenza). Senza questi metadati il chunk non entra nell'indice.

Le fasi attingono dalla fonte [Normattiva](/fonti/normattiva.md) e alimentano l'[indice normativo](/architettura/indice-normativo.md).
