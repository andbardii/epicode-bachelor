# Migrazione in epicode-bachelor

Migrazione del 13 ottobre 2026. Importazioni tramite `git subtree add`, senza `--squash` e senza riscrivere la cronologia. Gli hash originali restano invariati.

| Progetto | Repository originale | Branch | Commit importato | Tag |
| --- | --- | --- | --- | --- |
| [object-oriented-programming](object-oriented-programming/) | [andbardii/object-oriented-programming](https://github.com/andbardii/object-oriented-programming) | `main` | `9922bad11cb1c3754e96cffdac00a95ac475c5d3` | `migration/object-oriented-programming` |
| [data-structures-and-algorithms](data-structures-and-algorithms/) | [andbardii/data-structures-and-algorithms](https://github.com/andbardii/data-structures-and-algorithms) | `main` | `d989cb5fd4946c76e21ef45ee45969b1d53f2369` | `migration/data-structures-and-algorithms` |

## Consultare i commit originali

```sh
# Cronologia completa della raccolta e dei progetti importati
git log --all --graph --oneline

# Cronologia originale di un progetto, prima della migrazione
git log migration/object-oriented-programming

# Modifiche alla cartella dopo l’importazione
git log -- object-oriented-programming/
```

Prima dell’importazione i file erano nella radice delle singole repository: un filtro sul nuovo percorso non mostra da solo tutti i commit precedenti. Usa il tag di migrazione per consultarli con i percorsi originali.

Le repository sorgenti vengono conservate come archivi con un collegamento alla nuova posizione. Issue, pull request e release storiche rimangono nelle repository originali; non sono trasferite da un’importazione Git. Le licenze di ciascun progetto sono conservate.
