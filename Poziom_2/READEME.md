# Analiza danych COVID-19

## Opis projektu
Projekt dotyczy analizy danych COVID-19 dla 10 wybranych krajów w kwietniu 2021 roku. Dane obejmują liczbę nowych zachorowań, zgonów, szczepień, PKB, populację oraz wskaźniki demograficzne i gospodarcze.

## Cele analizy
- Porównanie liczby zachorowań, zgonów i szczepień w odniesieniu do PKB i populacji.
- Normalizacja danych na 1000 mieszkańców oraz względem populacji miejskiej.
- Analiza korelacji między wskaźnikami epidemiologicznymi, gospodarczymi i demograficznymi.

## Główne obserwacje

### 1. Analiza w odniesieniu do PKB
- Turcja, Polska, Węgry i Bułgaria wyróżniają się dużą liczbą zachorowań w stosunku do PKB.
- Bułgaria ma najwyższy stosunek zgonów do PKB.
- Węgry, Litwa, Chorwacja, Polska, Turcja i Grecja przodują w liczbie szczepień względem PKB.
- Rosja radziła sobie lepiej niż oczekiwano, mimo słabszego PKB per capita.

### 2. Analiza w odniesieniu do populacji
- Normalizacja danych pozwala lepiej ocenić sytuację epidemiologiczną.
- Turcja, Polska, Węgry i Bułgaria nadal wyróżniają się pod względem zachorowań.
- Węgry i Litwa osiągają bardzo wysoką średnią liczby szczepień na mieszkańca.

### 3. Normalizacja na 1000 mieszkańców
- Zachorowania: Turcja liderem, niespodzianka Chorwacja i Litwa.
- Zgony: Polska spada w rankingu w porównaniu do liczb bezwzględnych.
- Szczepienia: Węgry osiągają bardzo dobre wyniki po normalizacji, Rosja słabiej.

### 4. Normalizacja względem populacji miejskiej
- Chorwacja ma najwyższe zachorowania w miastach.
- W pozostałych przypadkach zmiany w rankingu są niewielkie.

### 5. Korelacje danych
- Między zachorowaniami, zgonami i szczepieniami korelacje dodatnie.
- Nowe zachorowania i zgony wykazują silniejsze powiązanie niż z szczepieniami.
- PKB per capita dodatnio koreluje ze szczepieniami, słabiej z zachorowaniami i zgonami.
- Wskaźniki demograficzne: gęstość zaludnienia ma niewielki wpływ na zachorowania i zgony.
- Obostrzenia: niewielkie dodatnie korelacje z zachorowaniami i zgonami.

## Technologie i biblioteki
- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn

## Wnioski
- Normalizacja danych jest kluczowa dla realistycznej oceny sytuacji epidemiologicznej.
- Turcja, Polska, Węgry i Bułgaria wyróżniają się pod względem zachorowań i zgonów.
- Wysoka liczba szczepień w Węgrzech, Litwie i Chorwacji jest pozytywnym zjawiskiem.
- Rosja osiągnęła lepsze wyniki niż oczekiwano przy niskim PKB per capita, co może wynikać z niskiej gęstości zaludnienia.
