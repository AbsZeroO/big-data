# Analiza danych COVID-19 – Regresja liniowa i wielomianowa
## Plik wynikowy final_level3

## Opis projektu
Projekt przedstawia analizę danych dotyczących pandemii COVID-19 w różnych krajach. W ramach analizy zastosowano regresję liniową oraz wielomianową w celu oceny dopasowania modeli do rzeczywistych danych. Analizowane dane obejmują:
- liczbę potwierdzonych przypadków,
- liczbę zgonów,
- liczbę szczepień,
- liczbę osób w pełni zaszczepionych,
- liczbę wykonanych testów.

Projekt podzielono na kilka części:
1. **Przygotowanie i wstępna eksploracja danych**  
2. **Regresja liniowa dla wybranych zmiennych**  
3. **Wnioski dotyczące ograniczeń regresji liniowej**  
4. **Regresja wielomianowa – dopasowanie modeli do danych Norwegii**  
5. **Porównanie regresji liniowej dla Włoch i Brazylii**  

---

## Część 2 – Regresja liniowa
Wykorzystano regresję liniową do modelowania m.in.:
- nowych pełnych szczepień,
- nowych testów.

### Wnioski:
Regresja liniowa nie oddaje dobrze dynamiki pandemii, gdyż:
- rozwój pandemii był **nieliniowy**,  
- duży wpływ miały czynniki zewnętrzne (np. decyzje polityczne, dostępność szczepionek),  
- modele nie uwzględniają opóźnień czasowych ani dynamicznych zmian.  

---

## Część 4 – Regresja wielomianowa
Dane dla **Norwegii** zostały przeanalizowane za pomocą regresji wielomianowej o stopniach od 1 do 15. Wyniki porównano z regresją liniową, korzystając z:
- **R²** – współczynnik determinacji,  
- **MSE** – błąd średniokwadratowy.  

### Wnioski:
- W każdym przypadku regresja wielomianowa osiągnęła **lepsze wyniki** niż liniowa.  
- Najlepiej dopasowane były:  
  - nowe zachorowania (**R² = 0,64**),  
  - nowe testy (**R² = 0,42**).  
- Szczepienia i pełne szczepienia osiągnęły gorsze dopasowanie, ale nadal lepsze niż regresja liniowa (**R² = 0,31 i 0,23**).  
- Najsłabiej dopasowane były dane o nowych zgonach (**R² = 0,07**), choć nadal lepsze niż w regresji liniowej.  

---

## Część 5 – Porównanie Włoch i Brazylii
Przeprowadzono analizę regresji liniowej w okresie od **27.12.2020 do 10.12.2021**. Dane podzielono na zbiór treningowy i testowy. Porównano:
- Włochy (Europa)  
- Brazylię (Ameryka Południowa)  

Uwzględniono również różnice w:
- PKB per capita,  
- gęstości zaludnienia,  
- udziale populacji miejskiej.  

### Wnioski:
1. **Nowe zachorowania** – Brazylia miała znacznie większe rozbieżności, co pokazuje słabszą kontrolę pandemii.  
2. **Nowe zgony** – liczba zgonów była znacznie wyższa w Brazylii, m.in. z powodu gorszej opieki zdrowotnej.  
3. **Nowe szczepienia** – w Brazylii wystąpił gwałtowniejszy wzrost liczby szczepień po starcie kampanii, choć Włochy rozpoczęły wcześniej (27.12.2020 vs. 17.01.2021).  
4. **Pełne szczepienia** – predykcje były do siebie zbliżone w obu krajach.  
5. **Nowe testy** – we Włoszech testów wykonywano więcej i stabilniej niż w Brazylii.  

---

## Podsumowanie
- **Regresja liniowa** nie jest odpowiednim narzędziem do modelowania danych o COVID-19, ze względu na nieliniowy charakter pandemii.  
- **Regresja wielomianowa** lepiej odwzorowuje trendy, choć jej skuteczność różni się w zależności od zmiennej.  
- Porównanie **Włoch i Brazylii** pokazuje, że różnice w gospodarce, opiece zdrowotnej i polityce miały znaczący wpływ na rozwój pandemii i skuteczność reakcji.  

---

📌 **Autorzy:**  
Projekt opracowany w ramach analizy danych COVID-19 z wykorzystaniem Pythona, bibliotek: `pandas`, `matplotlib`, `scikit-learn`.
"""
