---
title:   Mac nastavenie
isChild: true
anchor:  mac_setup
---

## Mac Nastavenie {#mac_setup_title}

OS X má predpripravené PHP, ale zvyčajte o niečo staršiu verziu než je aktuálna stabilná. Mountain Lion má
5.3.10, Mavericks má 5.4.17 a Yosemite má 5.5.9. Ale s aktuálným PHP 5.6 to to nie je dostatočné.

Existuje niekoľko spôsobov ako nainštalovať PHP na OS X.

### Inštalácia PHP pomocou Homebrew

[Homebrew] je výkonný balíčkovací manager pre OS X, ktorý Vám môže jednoducho pomôcť nainštalovať PHP
a rozličné rozšírenia. [Homebrew PHP] je repozitár, ktorý obsahuje PHP-prepojenú "formulae" pre Homebrew a dovolí
Vám nainštalovať PHP.

Momentálne môžete inštalovať `php53`, `php54`, `php55` alebo `php56` pomocou `brew install` príkazu a prepínať
medzi nimi pomocou modifikácie `PATH` premennej.

### Inštalácia PHP pomocou Macports

[MacPorts] Projekt je open-source komunitná iniciatíva pre prípravu ľahkopoužiteľného systému pre kompilovanie,
inštalovanie a aktualizovanie open-source softvéru pre OS X operačný systému či už na báze prikazového riadku,
X11 alebo Aqua rozhrania.

MacPorts podporuje pred-kompilované binárné súbory, čiže už nepotrebujete kompilovať všetky závislosti zo
zdrojových tarball súborov. Zachráni Vám to život ak nemáte žiaden balíček nainštalovaný na svojom operačnom
systéme.

Momentálne môžete inštalovať `php53`, `php54`, `php55` alebo `php56` pomocou `port install` príkazu, napríklad:

    sudo port install php54
    sudo port install php55

A môžete spustiť `select` príkaz pre prepnutie aktívneho php:

    sudo port select --set php php55

### Inštalácia PHP pomocou phpbrew

[phpbrew] je nástroj pre inštaláciu a správu viacero PHP verzií. Vie byť obzvlášť užitočný, ak 2 rozdielne
aplikácie/projekty potrebujú rozdielné verzie PHP a nepoužívate virtuálne stroje.

### Kompilácia zo zdroja

Ďalšia varianta, ktorá prináša možnosť výberu nainštalovanej PHP verzie je [samostatné kompilovanie][mac-compile].
V tom prípade si určite nainštalujte či už [Xcode][xcode-gcc-substitution] alebo Apple kompatibilné
["Command Line Tools for XCode"] voľné stiahnuteľné z Apple Mac Developer Center.

### All-in-One Inštalátory

Vyššie spomínané riešenia obsahujú hlavne samotné PHP a nedodávajú veci Apache, Nginx alebo SQL server.
"All-in-one" riešenia ako [MAMP][mamp-downloads] a [XAMPP][xampp] nainštalujú tieto ostatné časti ako ucelený
softvér. Táto jednoduchosť inštalácie ale prináša stratu flexibility.


[Homebrew]: http://brew.sh/
[Homebrew PHP]: https://github.com/Homebrew/homebrew-php#installation
[MacPorts]: https://www.macports.org/install.php
[phpbrew]: https://github.com/phpbrew/phpbrew
[mac-compile]: http://php.net/install.macosx.compile
[xcode-gcc-substitution]: https://github.com/kennethreitz/osx-gcc-installer
["Command Line Tools for XCode"]: https://developer.apple.com/downloads
[mamp-downloads]: http://www.mamp.info/en/downloads/
[xampp]: http://www.apachefriends.org/en/xampp.html
