# Tabelle Analitiche della Tesi di Dottorato

**Oggetto:** Quadro sinottico delle tabelle analitiche della tesi di dottorato (indice, contributi originali, produzione scientifica, analisi bibliografica)
**Autore:** Fabio Liberti — Dottorato in *Big Data e Intelligenza Artificiale*, Universitas Mercatorum (Ciclo XXXVIII), Matricola DT00200003
**Tesi:** *Federated Learning in Ambienti Dinamici ed Eterogenei per la Sanità Digitale Europea: Dal Framework Teorico all'Implementazione negli Ospedali Italiani*
**Data:** 30 giugno 2026
**Fonti:** TOC (`main.toc`), Cap 1 §1.7 (`tab:contributi_originali`), Cap 13 §13.1 (`tab:sintesi_risultati`), Appendice D, `bibliography/ref_master.bib` + `main.bbl` — versione congelata della tesi (submodule `foundations/tesi_fl_2025`, `main.pdf` 455 pagine).

> Documento analitico derivato (non fa parte della tesi). Estrazione automatizzata dalle fonti reali, nessun valore inventato.

**Firma:** _______________________________  (Fabio Liberti)

---

## 1. Tabella sintetica di indice

Tesi monografica — **455 pagine**, 4 Parti, 13 Capitoli + 5 Appendici.

| Parte | Cap. | Titolo | Pag. |
|---|---|---|---|
| **I — Introduzione e Stato dell'Arte** | 1 | Introduzione e Motivazioni della Ricerca | 5 |
| | 2 | Federated Learning nel Contesto Sanitario | 27 |
| | 3 | Standard e Framework Normativi | 39 |
| **II — Framework Teorico e Contributi** | 4 | Framework Teorico per FL Eterogeneo | 57 |
| | 5 | FENITH: Architettura Nazionale per il FL-EHDS | 73 |
| | 6 | AIDIGOSA: Governance Distribuita per il FL Sanitario | 99 |
| **III — Studi e Validazione Empirica** | 7 | Studio OPBGFL: applicazione EHDS+FL all'OPBG | 121 |
| | 8 | Studio BLEKFL2: collaborazione internazionale al BTH | 143 |
| | 9 | Validazione Empirica | 163 |
| | 10 | Indagine Nazionale sull'Adozione del FL | 195 |
| **IV — Discussione e Conclusioni** | 11 | Discussione Integrata | 233 |
| | 12 | Impatto, Sostenibilità e Raccomandazioni di Policy | 245 |
| | 13 | Conclusioni e Prospettive Future | 257 |
| **Appendici** | A | Dettagli Implementativi | 269 |
| | B | Dataset e Risultati Sperimentali | 287 |
| | C | Strumenti dell'Indagine Nazionale | 303 |
| | D | Pubblicazioni e Produzione Scientifica | 323 |
| | E | Documenti Amministrativi e Partnership | 339 |

**Legenda Tabella 1.** *Parte* = una delle quattro macro-sezioni in cui è articolata la tesi. *Cap.* = numero progressivo del capitolo (1–13) o lettera dell'appendice (A–E). *Titolo* = denominazione del capitolo/appendice come da indice. *Pag.* = pagina iniziale nel PDF compilato (455 pagine complessive). La struttura è di tipo **monografico** (tesi unitaria, non *paper collection*).

---

## 2. Tabella Risultati originali

Sintesi dei **5 contributi originali + 1 implementation guideline** (da `tab:sintesi_risultati`, integrata con `tab:contributi_originali`).

| Blocco | Risultato principale | Evidenza load-bearing | Paper | Cap. | RQ |
|---|---|---|---|---|---|
| **1 · Teorico** *(DHFLPL2)* | Formalizzazione eterogeneità multidim. + suite metriche adattive | FDI · RS · AR + **DEI** ∈[0,1]; analisi convergenza + garanzie privacy | **DHFLPL2**, **FL-EHDS** | 4 | RQ1 |
| **2 · Architetturale** *(FENITH)* | FENITH *reference architecture* EHDS-compliant | 5 layer + 2 framework; FHIR R5/OMOP; DP per-giurisdizione (Art. 48) + secure aggregation; TRL 4–9 | **FL-EHDS** | 3·5 | RQ1·RQ4 |
| **3 · Algoritmico** | Selezione algoritmica (semi-)automatica + *best-per-algorithm* | 17 algoritmi; 10/17 entro 3 pp da FedAvg; coordinamento 100% (DQN + **SharedStateManager**) | **FL-EHDS**, **XFL-STDF** | 8–9 | RQ1·RQ4 |
| **4 · Empirico** | Validazione su 4 *strand* + ecosistema sperimentale | **FL-EHDS** 6.004 esp.; ~7.960 ecosistema; 18 mesi + 6 mesi tirocinio | **FL-EHDS** + *monografici* (OPBGFL, BLEKFL2, Indagine Nazionale) | 7–10 | RQ1·RQ3 |
| **5 · Governance** *(AIDIGOSA)* | AIDIGOSA 4 dim. + 5ª organizzativa; modelli economici; policy | overhead governance <1,1%; Shapley Gini(SV) vs Gini(data) | **AIDIGOSA**, **FL-BMERN**, **FL-EHDS**, **FL-EHDSTAGE**, **FedHR5.0** | 6·12 | RQ2·RQ3 |
| **6 · Implementation guideline** | Incompatibilità Adam–SCAFFOLD (*boundary finding cross-dataset*) | +84,55 pp MNIST / +75,00 pp Fashion-MNIST; SCAFFOLD-specific | *boundary finding* | 7 | — |

**Legenda Tabella 2.** *Blocco* = i cinque contributi originali della tesi più l'*implementation guideline* conclusiva. *Risultato principale* = sintesi del contributo. *Evidenza load-bearing* = dato/risultato portante che sostiene il contributo. *Paper* = pubblicazioni peer-reviewed di riferimento (**in grassetto** = a prima firma dell'autore). *Cap.* = capitoli di sviluppo. *RQ* = *Research Question* servita.
*Sigle:* **DEI** = Diagnostic Equity Index (metrica originale, ∈[0,1]); **FDI** = Feature Drift Index; **RS** = Robustness Score; **AR** = Adaptation Rate; **DQN** = Deep Q-Network (apprendimento per rinforzo); **TRL** = Technology Readiness Level (scala 1–9); **DP** = Differential Privacy; **pp** = punti percentuali.
*Research Questions:* **RQ1** architetture *adaptive end-to-end* per l'eterogeneità multidimensionale e dinamica · **RQ2** modello di governance multi-stakeholder per il paradigma federato · **RQ3** evidenze empiriche sull'adozione nel Servizio Sanitario Nazionale · **RQ4** architettura *production-ready* EHDS-compliant con interoperabilità multi-livello.

---

## 3. Tabella paper

**7 peer-reviewed + 3 monografici (hard orphan) + 2 soft orphan** (da Appendice D §D.1).

| # | Sigla | Anno | Tipo | Venue / Sede | Ruolo autore | Cap. tesi |
|---|---|---|---|---|---|---|
| 1 | **OCI/DHFLPL2** | 2024 | Rivista (DOI) | *Applied Sciences* MDPI 14(18), 8490 | 1° autore (3 aut.) | 4·5·9 |
| 2 | **AIDIGOSA** | 2025 | Conf. (atti) | ItAIS 2025, Castellanza (IT) | 1° autore (7 aut.) | 6·4 |
| 3 | **FL-BMERN** | 2025 | Conf. (atti) | CIDE 2025, Ploiești (RO) | Autore unico | 3·6 |
| 4 | **XFL-STDF** | 2025 | Conf. (atti) | CIDE 2025, Ploiești (RO) | Co-autore (pres. Fanale) | 9·6 |
| 5 | **FL-EHDS** | 2026 | Conf. (in pubbl.) | FLICS 2026, Valencia (ES) | Autore unico | 5·9 |
| 6 | **FL-EHDSTAGE** | 2026 | Conf. (in pubbl.) | ICSIS 2026, Valencia (ES) | Autore unico | 11·12·6 |
| 7 | **FedHR5.0** | 2026 | Conf. (accettato) | IFKAD 2026, Budapest (HU) | Autore unico | 4·13 |
| 8 | OPBGFL | — | Monografico *(hard orphan)* | Tirocinio OPBG-IRCCS (18 mesi, Tozzi) | Autore | 7 |
| 9 | BLEKFL2 | — | Monografico *(hard orphan)* | Tirocinio BTH (6 mesi, Alawadi) | Autore | 8 |
| 10 | Indagine Nazionale | 2025 | Monografico *(hard orphan)* | OPBG — mixed-methods, Wave 1 giu–ago 2025 | Autore | 10 |
| — | FL-IDSADM | — | *Soft orphan* (sottomesso) | Reference arch. IDSA/Data Mesh EHDS | Autore | 13 (estensioni) |
| — | FL-FORGE | — | *Soft orphan* (workshop accettato, non pres.) | FL forense cross-dominio | Autore | 13 (nuovi domini) |

**Totali:** 7 peer-reviewed · 3 monografici · 2 soft orphan = **10 contributi principali** (+2).

**Legenda Tabella 3.** *Tipo* — **peer-reviewed** = contributo con revisione fra pari (rivista o atti di conferenza); **monografico (*hard orphan*)** = contributo autoriale privo di pubblicazione peer-reviewed dedicata, valorizzato nel corpo della tesi; **soft orphan** = iniziativa documentata per tracciabilità ma non computata fra i contributi scientifici attivi. *Ruolo autore* = posizione dell'autore nella *authorship*. *Cap. tesi* = capitoli in cui il contributo è mappato.
*Sedi/editori:* **MDPI** = Multidisciplinary Digital Publishing Institute · **ItAIS** = Italian Chapter of the Association for Information Systems · **CIDE** = Creativity and Innovation in Digital Economy · **FLICS** = Federated Learning and Intelligent Computing Systems · **ICSIS** = Sustainability, Innovation, and Society · **IFKAD** = International Forum on Knowledge Asset Dynamics · **OPBG-IRCCS** = Ospedale Pediatrico Bambino Gesù · **BTH** = Blekinge Institute of Technology (Karlskrona, SE).

---

## 4. Tabella analisi bibliografia — n = 451

Fonte: `bibliography/ref_master.bib` + `main.bbl` — **451 entries uniche** (voci stampate 1→451; `\bibentries` = 451; range anni 1912–2026).

### 4a — Classi di anno (n = 451)

| Classe | N. | % |
|---|---|---|
| ≤ 2010 | 36 | 8,0% |
| 2011–2015 | 16 | 3,5% |
| 2016–2018 | 63 | 14,0% |
| 2019–2020 | 76 | 16,9% |
| 2021–2022 | 102 | 22,6% |
| 2023 | 45 | 10,0% |
| 2024 | 46 | 10,2% |
| 2025 | 49 | 10,9% |
| 2026 | 18 | 4,0% |
| **Totale** | **451** | **100%** |
| *di cui recenti 2021–2026* | *260* | *57,6%* |

### 4b — Classi di tipologia (entry type) (n = 451)

| Tipo | N. | % |
|---|---|---|
| Articolo di rivista (`@article`) | 302 | 67,0% |
| Fonte web/istituzionale (`@misc`) | 69 | 15,3% |
| Atti di conferenza (`@inproceedings`) | 50 | 11,1% |
| Report tecnico (`@techreport`) | 20 | 4,4% |
| Libro (`@book`) | 7 | 1,6% |
| Altri (`@standard` / `@proceedings` / `@incollection`) | 3 | 0,7% |
| **Totale** | **451** | **100%** |

### 4c — Classi di argomento (n = 451)

*Classificazione tematica euristica sui titoli (il `.bib` non ha campo `keywords`); assegnazione a categoria prevalente con priorità — valori indicativi.*

| Argomento | N. | % |
|---|---|---|
| Federated Learning (metodi/algoritmi) | 114 | 25,3% |
| EHDS / Regolazione / Governance / Policy | 64 | 14,2% |
| Healthcare / Clinical AI / Imaging | 50 | 11,1% |
| Privacy / Sicurezza / DP / Byzantine | 43 | 9,5% |
| Standard / Interoperabilità (FHIR/OMOP/HL7) | 39 | 8,6% |
| AI in Management / Organizzazione / Business | 30 | 6,7% |
| Deep/Machine Learning generale | 22 | 4,9% |
| Metodologia ricerca (survey/case study) | 16 | 3,5% |
| Explainable AI / XAI | 11 | 2,4% |
| Education / Learning / Skills | 4 | 0,9% |
| Altro / fonti istituzionali (PNRR, decreti, ISTAT, GIMBE…) | 58 | 12,9% |
| **Totale** | **451** | **100%** |

**Legenda Tabella 4.** Analisi della bibliografia consolidata della tesi (**451 voci uniche**, numerate 1→451 nel PDF).
- **4a — Classi di anno:** distribuzione delle voci per fascia temporale, sulla base del campo `year`/`date` di ciascuna voce in `main.bbl`. La riga *recenti 2021–2026* misura l'attualità del corpus (57,6%). Dato **esatto**.
- **4b — Classi di tipologia:** distribuzione per *entry type* BibTeX. `@article` = articoli di rivista; `@inproceedings` = atti di conferenza; `@misc` = fonti web/istituzionali; `@techreport` = report tecnici; `@book` = libri. Dato **esatto**.
- **4c — Classi di argomento:** ripartizione tematica ottenuta per *matching* di parole chiave sui titoli, con assegnazione di ciascuna voce a **una sola** categoria (priorità per evitare doppi conteggi). Poiché il `.bib` non contiene un campo `keywords`, questa classificazione è **euristica e indicativa** (fotografia della composizione tematica, non dato bibliometrico certificato).
- *%* = percentuale sul totale di 451 voci.

---

### Note di rigore

- **Tabelle 1, 2, 3, 4a, 4b**: dati **esatti**, estratti dalle fonti reali (TOC, tabelle della tesi, Appendice D, `main.bbl`).
- **4a**: l'unica voce priva di campo anno/data (`fda2024meddev`) è assegnata al 2024 in base al citekey (documento FDA MEDDEV 2024).
- **4c**: classificazione **euristica/indicativa** (matching parole chiave sui titoli, una sola categoria per voce per priorità) — fotografia della composizione tematica, non dato bibliometrico certificato.

---

*Documento redatto in data 30 giugno 2026.*

**Firma:** _______________________________  (Fabio Liberti)
