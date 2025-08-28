# Analiza danych COVID-19 w PySpark 🧢💻

Projekt koncentruje się na eksploracji i analizie danych dotyczących pandemii COVID-19 z wykorzystaniem **PySpark**. Notebooki pokazują, jak łączyć, filtrować, agregować oraz wizualizować dane o krajach, populacji, gęstości zaludnienia, PKB, zakażeniach i szczepieniach.

---

## 🚀 Wymagania

Aby uruchomić projekt, potrzebujesz:

- Python 3.8+
- Apache Spark z biblioteką **PySpark**
- Plik danych wejściowych: `final_data.csv`

Instalacja PySpark:

```bash
pip install pyspark
```

## 🔎 Część 2 – Analiza danych COVID-19

W tej części skupiamy się na pliku final\_data.csv. Poniżej zwięzłe podsumowanie kluczowych kroków:

### Kluczowe działania

1. **Wczytywanie danych** – utworzenie sesji Spark, załadowanie CSV, konwersja kolumny date na typ daty.
2. **Definiowanie schematu** – ręczne określenie kolumn i selekcja interesujących danych.
3. **Tworzenie nowych kolumn** – np. `urban_population_ratio = population_urban / 2022 Population`.
4. **Łączenie informacji** – stworzenie kolumny `country_info` (nazwa kraju + kod + data).
5. **Filtrowanie danych** – wyodrębnienie krajów według PKB, populacji miejskiej, gęstości zaludnienia, liczby zgonów i szczepień.
6. **Agregacje** – liczba dni z dużą liczbą testów, suma szczepień, maksymalne przypadki, średnia liczba zgonów, globalne dane o szczepieniach.
7. **Analiza miesięczna** – sumowanie potwierdzonych przypadków per miesiąc.
8. **Łączenie danych (Joins)** – różne typy joinów do porównania i uzupełnienia zbiorów danych.

### Wyniki

Wyniki każdej operacji zapisano w osobnych folderach:

- `wyniki_2_6/` – filtrowania
- `wyniki_2_7/` – agregacje
- `wyniki_2_8/` – analiza miesięczna
- `wyniki_2_9/` – joins

## ✅ Podsumowanie

Projekt demonstruje praktyczne zastosowanie PySpark do analizy danych Big Data w kontekście COVID-19. Umożliwia:

- tworzenie nowych kolumn i metryk,
- filtrowanie i agregowanie danych,
- łączenie różnych zbiorów danych w elastyczny sposób.

Dzięki temu projekt stanowi kompletny przewodnik po analizie danych COVID-19 w PySpark 🌍.

