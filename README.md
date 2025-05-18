# ItalicAI – Dizionario Concettuale Italiano per l’AI e la Linguistica Computazionale

**ItalicAI** è il primo dizionario concettuale italiano compatto e “machine-ready”, progettato per l’intelligenza artificiale, la linguistica computazionale, la didattica e la ricerca.  
Basato su parsing e consolidamento automatico dei dati da Wiktionary e Morph-it,  
offre oltre 32.000 concetti atomici (sinonimi perfetti + forme flesse) in formato JSON,  
con meta compatibile NanoGPT e tool di traduzione open source.

## 🚀 Caratteristiche principali

- **Copertura totale:** Tutto il lessico italiano, senza rumore né duplicati.
- **Sinonimi perfetti:** Ogni token rappresenta un concetto puro e non ambiguo.
- **Forme flesse incluse:** Ogni lemma ha tutte le sue coniugazioni e varianti grammaticali.
- **Formato machine-friendly:** JSON e meta.pkl per pipeline AI, NLP e data science.
- **Pipeline e risultati trasparenti:** Preprint, dati, script (quando disponibili), meta e dizionario traduttore già pubblici.
- **Licenza IOK-NC:** Massima apertura per ricerca e sviluppo no-profit, protezione da abusi commerciali (arbitrato WIPO).

## 📦 Contenuto della cartella

```
ItalicAI/
│
├─ LICENSE.txt
├─ pre-publication_paper.pdf
├─ meta.pkl
├─ README.md
├─ tools/
├─ data/
     ├─ lista_forme-sinonimi.jsonl
     └─ lista_concetti.txt


## 🔥 Esempio d’uso Python

```python
import json

with open('concetti_completi.json', 'r', encoding='utf8') as f:
    concetti = json.load(f)

print(concetti["CONC_00123"]["sinonimi"])      # ['correre', 'sprintare', 'scattare']
print(concetti["CONC_00123"]["forme_flesse"])  # ['corro', 'corri', 'corre', ...]
```

## 📖 Documentazione e paper

Tutte le specifiche tecniche, dati e motivazioni sono descritte nel preprint allegato (`pre-publication_paper.pdf`).  
Il progetto è open a feedback, pull request, fork e proposte di collaborazione.

## 👨‍💻 Contatti

Autore: Samuele Scuglia  
Email: samuele.scuglia@gmail.com

## ⚖️ Licenza

Tutti i materiali sono distribuiti sotto la **Italica Open Knowledge & NonCommercial License (IOK-NC)**.  
Consultare `LICENSE.txt` per dettagli.  
Ogni controversia sarà risolta tramite arbitrato WIPO (Ginevra, lingua italiana).
