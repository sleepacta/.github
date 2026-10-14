# Come lavoriamo

Valido per tutte le repo di sleepacta.

## Ticket

- Ogni lavoro ha un'issue nella repo del codice che tocca, aperta con uno dei form: **Task**
  (il default), **Bug** o **Feature**. Basta il titolo.
- L'issue entra da sola nel Project [Sleepacta](https://github.com/orgs/sleepacta/projects/1):
  lì si imposta Sprint, Priorità, Area e assegnatario.
- Lo stato si cambia spostando la card nella Board (To Do, In Progress, Done). Una card in Done
  chiude l'issue; un'issue chiusa va in Done.
- Il numero dell'issue vale solo nella sua repo: per parlarne fuori da lì, "frontend #18" o il link.

## Commit

Una riga, il numero dell'issue davanti:

```
GH-18 Titolo
GH-18 Titolo, fixes #18      chiude l'issue quando il commit arriva sul branch di default
```

- `GH-18` e `#18` sono la stessa cosa per GitHub: link all'issue 18 di questa repo, e il commit
  compare nella issue. Va bene anche `#18 Titolo`, ma solo con `git commit -m`: in un editor
  (commit senza `-m`, amend, rebase, merge) git cancella le righe che iniziano con `#`.
- Ticket di un'altra repo: `sleepacta/exam-pipeline#12`.
- I commit vecchi con `SAWOR-NNNN` si riferiscono ai ticket Jira.
