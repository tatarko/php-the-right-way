---
title:  Formátovanie kódu
anchor: code_style_guide
---

# Formátovanie kódu {#code_style_guide_title}

PHP komunita je veľká a rôznorodá, poskladaná z nezpočítateľného množstva knižníc, frameworkov a komponentov. Bežne
PHP programátori vyberajú niekoľko z nich a kombinujú ich v jednom projekte. Je dôležité udržiavať PHP kód
(najviac ako sa dá) v spoločnom štýlovaní pre uľahčenie programátorom kombinovania viacaro knižníc v ich projektoch.

[Framework Interop Group][fig] navrhla a schvílila sériu odporúčaní štýlu. Nie všetky sú spojené zo samotným kódom,
ale tie, čo áno, sú [PSR-0][psr0], [PSR-1][psr1], [PSR-2][psr2] a [PSR-4][psr4]. Tieto odporúčania sú iba sadou
pravidiel, ktoré niektoré projekty ako Drupal, Zend, Symfony, CakePHP, phpBB, AWS SDK, FuelPHP, Lithium, atď
začínajú adaptovať. Môžete ich začaž používať vo vlatnom projekte alebo pokračovať vo svojom vlastnom štýle.

Ideálne by ste mali písať kód, ktorý udržiava známy štandard. Tým môže byť ľubovoľná kombinácia PSR alebo jedného
zo štandardov vytvorených PEAR-om alebo Zend-om. To znamená, že ostatní programátori môžu jednoducho čítať, pracovať
s vaším kódom a aplikácie, ktoré ho implementujú môžu mať konzistenciu aj pri práci s veľkým množstvom kódu tretích
strán.

* [Prečítajte si o PSR-0][psr0]
* [Prečítajte si o PSR-1][psr1]
* [Prečítajte si o PSR-2][psr2]
* [Prečítajte si o PSR-4][psr4]
* [Prečítajte si o PEAR Coding Standards][pear-cs]
* [Prečítajte si o Symfony Coding Standards][symfony-cs]

Môžete použiť [PHP_CodeSniffer][phpcs] pre skontrolovanie si kódu voči ľubovoľnému z týchto odporúčaní. Taktiež
existuje mnoho pluginov pre textové editory ako [Sublime Text 2][st-cs] pre poskytovanie živého feedbacku.

Automaticky môžete opraviť rozloženie kódu pomocou jedného z nástrojov. Jedným je [PHP Coding Standards Fixer][phpcsfixer],
ktorý je odtestovaný na dostatočne veľkej báze kódu. Ďalšou možnosťou je [php.tools][phptools], ktorý je známy vďaka
[sublime-phpfmt][sublime-phpfmt] pluginu. Nakoľko je novší s mnohými vylepšeniami vo výkone, poskytuje živé opravovanie
formátovania omnoho svižnejšie.

Angličtina je preferovaná pre všetky názvy symbolov a infraštruktúru kódu. Komentáre môžu byť napísané v ľubovoľnom jazyku
za predpokladu, že mu porozumejú všetci aktuálny a budúci používateľia využívajúci daný kód.


[fig]: http://www.php-fig.org/
[psr0]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md
[psr1]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md
[psr2]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md
[psr4]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-4-autoloader.md
[pear-cs]: http://pear.php.net/manual/en/standards.php
[symfony-cs]: http://symfony.com/doc/current/contributing/code/standards.html
[phpcs]: http://pear.php.net/package/PHP_CodeSniffer/
[st-cs]: https://github.com/benmatselby/sublime-phpcs
[phpcsfixer]: http://cs.sensiolabs.org/
[phptools]: https://github.com/dericofilho/php.tools
[sublime-phpfmt]: https://github.com/dericofilho/sublime-phpfmt
