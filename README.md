# Pirátský web Stredočeského kraje - stredocesky.pirati.cz

* soubory .md jsou v "Markdown" formátu - viz https://en.wikipedia.org/wiki/Markdown nebo https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
* pokud je to možné, je lepší použít md než html
* pokud kód nemůžete otestovat na lokále (stažení celého repa, build a spuštění v jekyllu), dělejte jen drobné změny, kterým rozumíte
* obecně k pirátským šablonám: https://github.com/pirati-web
* další repository pro inspiraci: https://github.com/pirati-web
* technická diskuze (nejen) k webu viz https://chat.pirati.cz/channel/stredocesi

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

