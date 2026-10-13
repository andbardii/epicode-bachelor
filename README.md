# EPICODE Bachelor

Materiali ed esercizi del mio percorso di laurea con EPICODE: programmazione a oggetti, strutture dati e algoritmi.

## Progetti

| Cartella | Contenuto | Tecnologie |
| --- | --- | --- |
| [object-oriented-programming](object-oriented-programming/) | Esercizi del percorso di laurea EPICODE dedicati alla programmazione a oggetti in Java. | Java |
| [data-structures-and-algorithms](data-structures-and-algorithms/) | Esercizi del percorso di laurea EPICODE su complessità, strutture dati e algoritmi in Python. | Python |

## Utilizzo

```sh
git clone https://github.com/andbardii/epicode-bachelor.git
cd epicode-bachelor
```

Ogni progetto mantiene la propria struttura e le proprie dipendenze. Consulta il README della cartella scelta per i percorsi di avvio; non esiste una build comune alla raccolta. Le versioni dei framework sono quelle dei progetti didattici originali.

## Cronologia e licenze

Le repository originali sono state importate con `git subtree`, senza squash: commit, autori, date e identificativi originali restano nella cronologia. I tag `migration/<nome-progetto>` identificano il punto di importazione. I riferimenti e i comandi di consultazione sono riportati sotto, nella sezione [Provenienza e cronologia](#provenienza-e-cronologia).

Ogni progetto conserva il proprio file `LICENSE` e le relative attribuzioni.

## Provenienza e cronologia

Migrazione del 13 ottobre 2026. Importazioni tramite `git subtree add`, senza `--squash` e senza riscrivere la cronologia. Gli hash originali restano invariati.

| Progetto | Repository originale | Branch | Commit importato | Tag |
| --- | --- | --- | --- | --- |
| [object-oriented-programming](object-oriented-programming/) | `andbardii/object-oriented-programming` | `main` | `9922bad11cb1c3754e96cffdac00a95ac475c5d3` | `migration/object-oriented-programming` |
| [data-structures-and-algorithms](data-structures-and-algorithms/) | `andbardii/data-structures-and-algorithms` | `main` | `d989cb5fd4946c76e21ef45ee45969b1d53f2369` | `migration/data-structures-and-algorithms` |

### Consultare i commit originali

```sh
# Cronologia completa della raccolta e dei progetti importati
git log --all --graph --oneline

# Cronologia originale di un progetto, prima della migrazione
git log migration/object-oriented-programming

# Modifiche alla cartella dopo l’importazione
git log -- object-oriented-programming/
```

Prima dell’importazione i file erano nella radice delle singole repository: un filtro sul nuovo percorso non mostra da solo tutti i commit precedenti. Usa il tag di migrazione per consultarli con i percorsi originali.

Le repository sorgenti sono state eliminate dopo la verifica dell’importazione. Un’importazione Git conserva commit e file, ma non trasferisce issue, pull request e release su GitHub. Le licenze di ciascun progetto sono conservate.
