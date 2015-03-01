---
title:   Paradigmy programovania
isChild: true
anchor:  programming_paradigms
---

## Paradigmy programovania {#programming_paradigms_title}

PHP je flexibilný, dynamický jazyk, ktorý podporuje rôzné programátorské techniky. Rokmi sa dramaticky vyvíjal,
najmä pridaním solídneho objektového programovania v PHP 5.0 (2004), anomných funkcií a namespacov v PHP 5.3
(2009) a trait-ami v PHP 5.4 (2012).

### Objektovo-orientované programovanie

PHP obsahuje kompletnú sadu objektovo-orientovaných vlastností vrátané tried, abstraktných tried, rozhraní, 
dedičností, konštruktorov, klonovania, výnimiek a ďalších.

* [Prečítajte si o Objektovo-orientovanom PHP][oop]
* [Prečítajte si o Traitoch][traits]

### Funkcionalné programovanie

PHP podporuje funkcie prvej triedy, čo znamená, že funkcia môže byť priradená premennej. Používateľom definované
aj zabudované funkcie môžu byť referencované premennou a zavolané dynamicky. Funkcie môžu byť predané ako
ako argumenty do iných funkcií a (vlastnosť nazývaná _Funkcie vyššieho rádu_) a funkcia môže navrátiť iné funkcie.

Rekurzia, vlastnosť jazyku, ktorá dovoľuje funkcií zavolať seba samú je podporovaná, ale vačšina PHP kódu
sa sústredí na iteráciu.

Nové anonymné funkcie (spolu s podporou closure) sú dostupné od verzie PHP 5.3 (2009).

PHP 5.4 pridalo možnosť spútať anonymnú funkciu s objektom a okrem toho ešte vylepšilo podporu pre volateľné premenné
tak, aby boli použiteľné rovnako ako anonymné funkcie v takmer všetkých prípadoch.

* Pokračujte v čítani o [Funkcionálnom programovaní v PHP](/pages/Functional-Programming.html)
* [Prečítajte si o anonymných funkciách][anonymous-functions]
* [Prečítajte si o Closure triede][closure-class]
* [Viac detailov v Closures RFC][closures-rfc]
* [Prečítajte si o Callables][callables]
* [Prečítajte si o dynamickom volaní funkcií pomocou `call_user_func_array()`][call-user-func-array]

### Meta programovanie

PHP podporuje viacero foriem meta-programovania pomocou mechanizmov ako Reflection API and Magické metódy. Existuje
mnoho magických metód ako `__get()`, `__set()`, `__clone()`, `__toString()`, `__invoke()`, atď., ktoré dovoľujú
programátorom ovplyvniť správanie triedy. Ruby programátori často hovoria, že PHP chýba `method_missing`, ale
tá je dostupná ako `__call()` a `__callStatic()`.

* [Prečítajte si o magických metódach][magic-methods]
* [Prečítajte si o reflekcií][reflection]
* [Prečítajte si o preťažení][overloading]


[oop]: http://php.net/language.oop5
[traits]: http://php.net/language.oop5.traits
[anonymous-functions]: http://php.net/functions.anonymous
[closure-class]: http://php.net/class.closure
[closures-rfc]: https://wiki.php.net/rfc/closures
[callables]: http://php.net/language.types.callable
[call-user-func-array]: http://php.net/function.call-user-func-array
[magic-methods]: http://php.net/language.oop5.magic
[reflection]: http://php.net/intro.reflection
[overloading]: http://php.net/language.oop5.overloading

