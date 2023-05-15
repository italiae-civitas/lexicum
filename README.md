# Lexicum

![GitHub](https://img.shields.io/github/license/urbs-italiae/lexicum?style=for-the-badge)
![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/urbs-italiae/lexicum?sort=semver&style=for-the-badge)
![Packagist Dependency Version](https://img.shields.io/packagist/dependency-v/urbs-italiae/lexicum/drupal/core-recommended?style=for-the-badge)
![Packagist Downloads](https://img.shields.io/packagist/dt/urbs-italiae/lexicum?style=for-the-badge)

[Lexicum](https://www.grecoantico.com/dizionario-greco-antico.php?parola=lexikon) è un modulo Drupal che installa i vocabolari utilizzati dai Comuni.
Lexicum, oltre ai vocabolari, importa le configurazioni degli url.

## Requisiti
- Drupal: >= 10
- Profilo Drupal: `minimal`
- Moduli contrib: `pathauto`

## Installazione
Per aggiungere il modulo alla tua installazione esegui:
```shell
$ composer require drupal/pathauto urbs-italiae/lexicum
```
Installa il modulo `pathauto` e configuralo:
```shell
$ drush -y pm:install pathauto
$ drush -y config:set pathauto.settings punctuation.slash 1
```
Infine, installa Lexicum
```shell
$ drush -y en lexicum
```

Questo è il risultato:

![Screenshot con l'elenco dei vocabolari installati](docs/vocabolari.png "Screenshot con l'elenco dei vocabolari installati")

## Moduli consigliati
Per importare le voci di tassonomia nei vocabolari puoi usare:
[Congruere lexicum](https://github.com/urbs-italiae/congruere_lexicum)

## License

Copyright (C) 2023 https://github.com/urbs-italiae

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License version 3 as published by the Free Software Foundation.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

Questo è un software libero: puoi ridistribuirlo e/o modificarlo secondo i termini della GNU General Public License versione 3 pubblicata dalla Free Software Foundation.

Questo programma è distribuito nella speranza che possa essere utile, ma SENZA ALCUNA GARANZIA; senza nemmeno la garanzia implicita di COMMERCIABILITÀ o IDONEITÀ PER UNO SCOPO PARTICOLARE. Vedere la GNU General Public License per maggiori dettagli.
