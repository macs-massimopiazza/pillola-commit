# Guida "[conventional commit](https://www.conventionalcommits.org/en/v1.0.0/)"
## Scrivere messaggi di commit descrittivi e rilevanti

> 🚨 Disclaimer
> 
> La convenzione che decidete di usare varia da più fattori: preferenze soggetive, grandezza del progetto, da quante persone ci lavorano, etc.
>
> Noi vi mostreremo una delle più comuni, che può andare bene per la maggior parte delle situazioni.
>
> Potete cambiarne qualche aspetto a seconda delle vostre preferenze.
>
>L'importante è scegliere una convenzione ed essere consistenti, usandola quindi per tutto il progetto (nel vostro caso l'esercizio).

## Basi di Semantic Code Versioning

`MAJOR`.`MINOR`.`PATCH`
- `MAJOR` detto anche breaking change. Quando le modifiche rendono **NON** retrocompatibile il codice.
- `MINOR` Aggiunta di una feature (aggiuntà di nuova funzionalità). Retrocompatibili con il codice
- `PATCH` Risoluzione di bug e modifiche che non aggiungono funzionalità specifiche. Retrocompatibili con il codice

### Commit history che vogliamo evitare

![commit con type, scope e description](/img/bad-commit-history.png)

## Sintassi di base

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Obbligatori
```<type>```
- **Comunica l'intendo della modifica** 
- type più comuni: `fix`, `feat` <small>check angular convention</small>

```<description>```
- **Breve messaggio che descrive cosa fa la commit**
- scritto in imperativo (usare add invece di adds o added)

### Opzionali
```[optional scope]```
- **Qualsiasi informazione aggiuntiva**
- usare sostantivi, nomi
- `!` se si tratta di breaking changes

```[optional body]```
- **Descrive che modifiche hai fatto e perchè le hai fatte**
- forma libera
- solo le commit più complesse lo necessitano (raro per i progetti ed esercizi personali)

```[optional footer(s)]```
- **Informazioni aggiuntive**
- per specificare la issue a che risolve
- per aggiungere metadati

## Esempi di commit history
### Esercizio Fizzbuzz

```
build: add base project files

feat: show numbers from 1 to 100 in console

feat: replace mutiples matching numbers with related keyword (fizz, buzz, fizzbuzz)

fix: avoid if statement never check fizzbuzz condition (multiples of 3 & 5)
Base exercise completed

feat(bonus 1): show box with number/keyword on page (instead of console)

feat(bonus 2): style box according to its content (number or keyword)

style: remove blank spaces and unecessary code
```

<br>

![commit con type e description](/img/commit-1.png)
<br>

![commit con type, description e footer](/img/commit-2.png)
<br>

![commit con type, scope e description](/img/commit-3.png)
