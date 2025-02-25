# Představení projektu
Bakalářská práce se zabývá použitím CV (computer vision) ve stavebnictví, konkrétně orientačním výpočtem tepelné ztráty z fotografie fasády.

Vstupem je fotografie fasády budovy, výstupem je orientační výpočet tepelné ztráty. Výpočet se skládá z následujících prvků:
- segmentace fasády a jednotlivých prvků (zdivo, střecha, okna, dveře) z fotografie,
- extrakce dat z katastru nemovitostí
	- výměra pozemku
	- aproximace pomocí obdélníku
- spojení dat z fotografie a katastru a následný výpočet *pixel-per-meter* poměru ve fotografii
- výpočet ploch jednotlivých prvků fasády
- aproximovaný výpočet tepelné ztráty pomocí středních hodnot U-value (tj. reciproké hodnotě tepelného koeficientu)

# Cílová skupina
Majitelé nemovitostí, kteří chtějí zjistit orientační výpočet tepelné ztráty svého domu, nebo mají dlouhou čekací lhůtu na EKIS konzultaci. Chtějí předběžně zjistit, jestli je jejich dům vhodný na zateplení, společně s orientačním výpočtem úspory nákladů při zateplení nebo jiných doporučených úsporných opatřeních (např. s tepelným čerpadlem).

# Návod k používání
Návod pro uživatele by měl obsahovat:
- jak správně vyfotit fasádu, aby byla přesnost výpočtu co nejvyšší
- jak nahrát fotografii do aplikace
- jak vybrat focenou fasádu z obdélníku na fotografii (pro výpočet *pixel-per-meter* poměru)
- jak interpretovat výsledky výpočtu
- jaké jsou limity výpočtu a jaké jsou případné chyby
- jaké jsou další kroky po získání výsledků, např.
	- kontakty na EKIS konzultanty v okolí
	- kontakty na zateplovací (a tepelnočerpadlářské) firmy v okolí

## Forma návodu
Jelikož bude aplikace webová, bude návod k používání také ve formě webové stránky. Stránka bude obsahovat:
- instruktážní video
- textový popis u každého kroku
- možnost stáhnutí návodu s textovým popisem a instruktážními videi ve formátu PDF
	- vhodná i pro distribuci EKIS konzultanty a zateplovacími firmami