---
title:   Windows nastavenie
isChild: true
anchor:  windows_setup
---

## Windows nastavenie {#windows_setup_title}

PHP je na Windowse dostupné vo viacerých spôsoboch. Môžete si [stiahnuť binárné súbory][php-downloads] a donedávna
ste mohli používať '.msi' inštalátor. Ten už ale nie je naďalej podporovaný a končí na verzií PHP 5.3.0.

Pre učenie a lokálny vývoj môžete použiť zabudovaný webserver s PHP 5.4+, čiže nemusíte si robiť starosti s jeho
nastavovaním. Ak preferujete "all-in-one" riešenie, ktoré zahŕňa plnohodnotný webserver a tiež MySQL, tak nástroje
ako [Web Platform Installer][wpi], [XAMPP][xampp], [EasyPHP][easyphp] a [WAMP][wamp] pomôžu rýchlo rozbehať
fungujúci Windows vývojoví environment. Je ale nutné dodať, že tieto nástroje budú o niečo odlišné voči produkčným,
čiže buďte opatrní voči rozdielmi prostredí v prípade, že vývijate na Windowse a deployujete na Linux.

Ak potrebujete v produkcií bežať na Windowse, tak IIS7 Vám poskytne najstabilnejší a najlepší výkon. Môžete používať
[phpmanager][phpmanager] (GUI plugin pre IIS7) pre jednoduché nastavovanie a správu PHP. IIS7 obsahuje zabudované
FastCGI pripravené bežať. Potrebujete iba nakonfigurovať PHP ako handler. Pre podporu a ďalšie informácie
existuje [samostatná časť na iis.net][php-iis] pre PHP.


[php-downloads]: http://windows.php.net
[wpi]: http://www.microsoft.com/web/downloads/platform.aspx
[xampp]: http://www.apachefriends.org/en/xampp.html
[easyphp]: http://www.easyphp.org/
[wamp]: http://www.wampserver.com/en/
[phpmanager]: http://phpmanager.codeplex.com/
[php-iis]: http://php.iis.net/
