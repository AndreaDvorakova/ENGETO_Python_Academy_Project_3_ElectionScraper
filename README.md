# Election Scraper

## Popis projektu

Tento projekt slouží k extrahování výsledků z parlamentních voleb 2017. Odkaz k prohlédnutí [zde](https://volby.cz/pls/ps2017nss/ps3?xjazyk=CZ).

## Instalace knihoven

Knihovny, které jsou použity v kódu jsou uložené v souboru ```requirements.txt```. Pro instalaci doporučuji použít nové virtuální prostředí a nainstalovaným manažerem spustit následovné:

```ruby
$ pip3 -- version                       # overim verzi manazera
$ pip3 install -r requirements.txt      # nainstalujeme knihovny
```

## Souštění projektu

Spuštění souboru ```main.py``` v rámci příkazového řádku požaduje dva povinné argumenty.

```ruby
python main.py <odkaz-uzemniho-celku><vysledny-soubor>
```
Následně se vám stáhnou výsledky, jako soubor s příponou ```.csv```.

## Ukázka projektu

Výsledky hlasování pro okres Bruntál:

1. argument: ```https://volby.cz/pls/ps2017nss/ps32?xjazyk=CZ&xkraj=14&xnumnuts=8101``` 
2. argument: ```vysledky_bruntal.csv```

Souštění programu:

```python main.py 'https://volby.cz/pls/ps2017nss/ps32?xjazyk=CZ&xkraj=14&xnumnuts=8101' vysledky_bruntal.csv```

