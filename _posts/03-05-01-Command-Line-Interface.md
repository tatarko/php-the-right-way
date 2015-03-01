---
title:   Rozhranie príkazového riadku
isChild: true
anchor:  command_line_interface
---

## Rozhranie príkazového riadku {#command_line_interface_title}

PHP bolo vytvorené pre písaní webových aplikácií, ale je použiteľné aj pre skriptovanie rozhraní príkazového riadku
(CLI). Programy príkazového riadku môžu napomôcť automatizovať bežné veci ako testovanie, deployment a aministrácia
aplikácií.

CLI PHP programy sú užitočné preto, lebo môžete využívať kód vašej aplikácie bez potreby vytvárania a zabezpečovania
webového GUI. Len samozrejme **nedávajte** vaše CLI PHP skripty do vášho verejného web priečinku!

Vyskúšajte spustiť PHP z príkazového riadku:

{% highlight console %}
> php -i
{% endhighlight %}

Prepínač `-i` vypíše vašu PHP konfiguráciu podobne ako [`phpinfo()`][phpinfo] funkcia.

Prepínač `-a` ponúka interaktívny shell podobný IRB od ruby alebo python-ovému interaktívnemu shellu. Okrem toho
existuje ešte množstvo užitočných [prepínačov prákazového riadku][cli-options].

Napíšme jednoduchý "Hello, $name" CLI program. Pre vyskúšanie vytvorte súbor pomenovaný `hello.php` ako nižšie.

{% highlight php %}
<?php
if ($argc !== 2) {
    echo "Usage: php hello.php [name].\n";
    exit(1);
}
$name = $argv[1];
echo "Hello, $name\n";
{% endhighlight %}

PHP nastaví dve špeciálne premenné na základe argumentov, s ktorými spustíte svoj skript. [`$argc`][argc] je číselná
premenná obsahujúca *počet* argumentov and [`$argv`][argv] je pole obsahujúce hodnotu *každého* argumentu.
Prvý argument je vždy názov vášho PHP skriptu, v tomto prípade `hello.php`.

Výraz `exit()`  sa používa s nenulovou hodnotou na to, aby shell vedel, že príkaz skončil chybou. Často používané
exit kódy môžete nájsť [tu][exit-codes].

Pre spustenie nášho skriptu vyššie z príkazového riadku:

{% highlight console %}
> php hello.php
Usage: php hello.php [name]
> php hello.php world
Hello, world
{% endhighlight %}


 * [Priučte sa spúšťaniu PHP z príkazového riadku][php-cli]
 * [Priučte sa nastaveniu Windowsu na spustenie PHP z príkazového riadku][php-cli-windows]


[phpinfo]: http://php.net/function.phpinfo
[cli-options]: http://php.net/features.commandline.options
[argc]: http://php.net/reserved.variables.argc
[argv]: http://php.net/reserved.variables.argv
[exit-codes]: http://www.gsp.com/cgi-bin/man.cgi?section=3&amp;topic=sysexits
[php-cli]: http://php.net/features.commandline
[php-cli-windows]: http://php.net/install.windows.commandline
