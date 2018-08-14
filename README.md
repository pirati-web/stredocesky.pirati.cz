# Pirátský web Stredočeského kraje - stredocesky.pirati.cz

* pokud je to možné, je lepší použít Markdown (.md) formát než html
* pokud kód nemůžete otestovat na lokále (stažení celého repa, build a spuštění v jekyllu), dělejte jen drobné změny, kterým rozumíte
* obecně k pirátským šablonám: https://github.com/pirati-web
* další repository pro inspiraci: https://github.com/pirati-web
* technická diskuze (nejen) k webu viz https://chat.pirati.cz/channel/stredocesi

# Co má nebo musí mít článek

* jméno článku rozumné délky
* autora
* datum (pokud nemá být aktuální)
* titulní fotografii (zobrazuje se v seznamu článků a také v samotném článku nahoře - bez dalšího popisu)
* tagy
* text co nejméně formátovaný + případně další fotografie

# Co má nebo musí mít osobní profilová stránka

* jméno a příjmení, tituly
* u piráta uživatelské uid
* kontakt (minimálně pirátský e-mail), případně linky na osobní weby atd.
* fotka (hlava) - ořezává se do čtverce a nechává se v co nejvyšším rozlišení
* historie vč. data a místa narození, profese a záliby

# Markdown formát

```
# Nadpis
## Menší nadpis
*kurzíva* **tučné písmo** ~~škrtance~~ `kód`
* seznam nečíslovaný
1. seznam číslovaný
[odkaz](http://www.pirati.cz)
```

Jak správně citovat:

```
> „Tohle říkám."
říká Petr Novák.
```

Více viz https://en.wikipedia.org/wiki/Markdown nebo https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

# Jednoduchá editace souborů přímo na githubu

Pro editaci stačí mít github účet, nejsou potřeba žádná speciální práva. Postup je následující:

1. ...
2. ...

# Pro linuxáky

Vystačíte si s jakýmkoliv editorem a "git" klientem (balík by se měl jmenovat stejně). Pár tipů pro command line git klienta viz níže - i tak byste ale měli vědět, co v každém kroku děláte!

Více viz https://help.github.com/


## Start

```
mkdir ~/git
cd ~/git
git clone https://github.com/pirati-web/stredocesky.pirati.cz
git config user.name "vas_github_user"
git config --global credential.helper cache
git config --global credential.helper 'cache --timeout=3600'
```

## Zápis změn do lokálního repository a přenos na server

```
git status
git add -A
git commit -a
git push
```

## Aktualizace lokálního repository

To udělejte vždy, než něco začnete měnit.

```
git fetch
```
