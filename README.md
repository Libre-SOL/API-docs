# Neoficiální dokumentace API Škola OnLine

Tento repozitář obsahuje technickou specifikaci REST API školního systému Škola OnLine. Dokumentace byla vytvořena na základě analýzy síťového provozu (reverse engineering) a je zpracována ve standardu OpenAPI 3.0.

## Online dokumentace

Interaktivní dokumentace je hostována pomocí GitHub Pages a využívá Swagger UI pro vizualizaci.

**Odkaz na dokumentaci:**
https://libre-sol.github.io/API-docs/

## Obsah repozitáře

* **dokumentace.yaml**
  Hlavní soubor s definicí API ve formátu OpenAPI 3.0. Obsahuje popisy endpointů pro autentizaci, získání informací o uživateli, známek, rozvrhu a domácích úkolů.

* **index.html**
  Statická HTML stránka, která načítá knihovnu Swagger UI a soubor `dokumentace.yaml`.


## Lokální spuštění

Pokud si chcete prohlédnout dokumentaci lokálně, nelze soubor `index.html` otevřít přímo v prohlížeči kvůli omezení CORS (načítání lokálního YAML souboru). Je nutné spustit lokální HTTP server.

1. Otevřete terminál ve složce repozitáře.
2. Spusťte Python HTTP server:
   ```bash
   python -m http.server 8000