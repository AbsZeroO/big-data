# Podstawy Przetwarzania Dużych Zbiorów Danych – Projekt COVID-19

Projekt realizowany w ramach zajęć **Podstawy Przetwarzania Dużych Zbiorów Danych**.  
Autorzy:  
- Łukasz Moskwa
- Artur Szewczykowski

## 📌 Opis
Celem projektu jest zapoznanie się z narzędziem **Google BigQuery** oraz wykorzystanie publicznych zbiorów danych związanych z pandemią COVID-19. Notebook zawiera przykłady połączenia z BigQuery, pobierania danych do Pythona (DataFrame Pandas) oraz ich podstawowej eksploracji i analizy.

Źródła danych:  
- [COVID-19 Open Data](https://github.com/GoogleCloudPlatform/covid-19-open-data)  
- [Dokumentacja tabeli](https://github.com/GoogleCloudPlatform/covid-19-open-data/blob/main/docs/table-by-sex.md)  

## ⚙️ Wymagania
- Python 3.8+
- Konto Google Cloud z dostępem do **BigQuery**
- Plik z kluczem JSON do usługi (Google Cloud Service Account)

Biblioteki używane w projekcie:
- `pandas`
- `google-cloud-bigquery`

## 🚀 Uruchomienie
1. Sklonuj repozytorium lub pobierz notebook `Poziom1.ipynb`.
2. Skonfiguruj środowisko wirtualne i zainstaluj wymagane paczki:
   ```bash
   pip install pandas google-cloud-bigquery
   ```
3. Pobierz plik klucza JSON z Google Cloud i umieść go w katalogu `.env/`.
4. Ustaw zmienną środowiskową w notebooku:
   ```python
   os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = ".env/<nazwa_pliku>.json"
   ```
5. Uruchom notebook w Jupyter Lab / Jupyter Notebook:
   ```bash
   jupyter notebook Poziom1.ipynb
   ```

## 📊 Zakres analizy
Notebook obejmuje:
- konfigurację klienta BigQuery,
- pobranie przykładowych danych z tabeli COVID-19,
- podstawowe zapytania SQL (m.in. liczba rekordów, liczba krajów),
- eksplorację i wstępną analizę zbioru.

## 📂 Struktura projektu
```
.
├── Poziom1.ipynb   # Notebook z analizą
├── .env/           # Katalog z kluczem JSON (nie dołączony do repo)
└── README.md       # Dokumentacja projektu
```

## 📝 Uwagi
- Plik z kluczem JSON do Google Cloud **nie jest dołączony** do repozytorium. Każdy użytkownik musi wygenerować własny.
- W przypadku problemów z dostępem do danych należy upewnić się, że w Google Cloud aktywowano **BigQuery API**.
