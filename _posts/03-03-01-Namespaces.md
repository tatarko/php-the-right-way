---
title:   Menné priestory
isChild: true
anchor:  namespaces
---

## Menné priestory - Namespaces {#namespaces_title}

Ako bolo spomenuté vyššie, PHP komunita má mnoho programátorov programátorov vytvárajúcich množstvo kódu. To znamená
jedna knižnica môže použiť rovnaký názov triedy ako iná knižnica. Keď sú tieto knižnice použité v jednom projekte,
môžu spôsobiť kolíziu a s tým súvisiace problémy.

_Namespaces (menné priestory)_ riešia tento problém. Ako je opísané v PHP manuále, menné priestory môžu byť prirovnané
k priečinkom operačného systému, ktorý _pomenúvava_ súbory; dva súbory s rovnakým názvom môžu existovať v rozdielnych
priečinkoch. Podobne dve PHP triedy môžu existovať rovnakým spôsobom v oddelených PHP menných priestoroch. Je to tak jednoduché.

Je dôležité, aby ste vlastný kód dávali do samostatného menného priestoru, aby mohol byť následne použitý inými programátormi
bez obáv z kolízie s inými knižnicami.

Jeden odporúčaný spôsob ako pomenovať vlastný menný priestor je opísaný v [PSR-4][psr4], ktorý cieli o vytvorenie spoločnej
konvencie pre pomenovanie súboru, triedy a menného priestoru pre vznik plug-and-play kód.

V Októbri 2014 PHP-FIG nechal zastarnúť predchadzajúci štandard: [PSR-0][psr0], ktorý bol nahradený novším [PSR-4][psr4].
Momentálne sú obe používané nakoľko PSR-4 vyžaduje PHP 5.3 a mnoho PHP 5.2 projektov preto využíva PSR-0. Ak sa chystáte
používať autoloading štandard pre novšiu aplikíciu alebo balíček, tak potom sa takmer určite chcete pozrieť na PSR-4.

* [Prečítajte si o menných priestoroch][namespaces]
* [Prečítajte si o PSR-0][psr0]
* [Prečítajte si o PSR-4][psr4]


[namespaces]: http://php.net/language.namespaces
[psr0]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md
[psr4]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-4-autoloader.md
