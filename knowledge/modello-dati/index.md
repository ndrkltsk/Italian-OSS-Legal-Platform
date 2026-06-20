---
type: Indice
title: Modello dati e parsing Akoma Ntoso
description: Come la piattaforma rappresenta una norma italiana a partire da Normattiva (Akoma Ntoso / ELI) e la trasforma in unità interrogabili.
tags: [modello-dati, akoma-ntoso, eli, rag]
timestamp: 2026-06-18T00:00:00Z
---

# Modello dati e parsing Akoma Ntoso

Questa cartella descrive come Magistra rappresenta una norma italiana a partire dai dati di Normattiva ([Akoma Ntoso](/glossario/akoma-ntoso.md) / [ELI](/glossario/eli.md)) e come la trasforma in unità interrogabili per la ricerca semantica e le citazioni.

> È una **bozza concettuale**: lo schema serve a ragionare sui dati, non è ancora un'implementazione.

## Concetti di base

- [Il modello FRBR](/modello-dati/frbr.md) — Work / Expression / Manifestation / Item.
- [Identificazione: URI ELI](/modello-dati/uri-eli.md) — chiave primaria stabile.
- [Struttura del documento AKN](/modello-dati/struttura-akn.md) — articolo e comma.
- [Pipeline di trasformazione](/modello-dati/pipeline-trasformazione.md) — da Normattiva all'indice vettoriale.

## Entità del modello dati interno

- [Norma](/modello-dati/norma.md) (Work)
- [Versione](/modello-dati/versione.md) (Expression)
- [Unità](/modello-dati/unita.md) (articolo / comma)
- [Chunk](/modello-dati/chunk.md) (ricerca semantica)
- [Riferimento](/modello-dati/riferimento.md) (cross-reference)
