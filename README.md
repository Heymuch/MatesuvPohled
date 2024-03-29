# Matesův Pohled
Zdrojové kódy pro web 'Matesův pohled'

## Požadované funkce
### Příspěvky
- [ ] Vytvoření a správa příspěvků
- [ ] Přiřazení jednotlivých příspěvků do kategorií
- [ ] Přiřazení značek (tagů) k příspěvku
- [ ] Možnost plánovaného uveřejnění příspěvku
- [ ] Generování odkazů ke sdílení příspěvků na sociální sítě (Facebook, Twitter, ...)
- [ ] Sledování návštěvnosti jednotlivých příspěvků
- [ ] Diskuze pod jednotlivými příspěvky

### Uživatelé a skupiny
- [ ] Vytvožení a správa uživatelů/skupin

### Administrace
* Přihlášení uživatele
* Správa stránek

## Datová struktura
### Příspěvek
| Název sloupce | Datový typ | Popis                         |
| ------------- | ---------- | ----------------------------- |
| id            | UUID       | Unikátní identifikátor článku |
| author\_id    | UUID       | Unikátní identifikátor autora |
| header        | String     | Nadpis článku                 |
| body          | String     | Obsah článku                  |
| created       | Datetime   | Datum vytvoření článku        |
| published     | Datetime   | Datum publikování článku      |

### Příspěvek > Kategorie
| Název sloupce | Datový typ | Popis                                     |
| ------------- | ---------- | ----------------------------------------- |
| id            | UUID       | Unikátní identifikátor kategorie          |
| name          | String     | Název kategorie                           |
| short\_name   | String     | Zkrácený název kategorie                  |
| description   | String     | Popis kategorie                           |
| enabled       | Boolean    | Možnost přidávat do kategorie nové články |
| created       | Datetime   | Datum vytvoření kategorie                 |
