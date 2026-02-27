# Adult Census Income Prediction
##  O projekcie
Celem tego projektu jest zbudowanie modelu uczenia maszynowego (klasyfikacja binarna), który przewiduje, czy roczny dochód danej osoby przekracza 50,000 USD. Analiza oparta jest na danych demograficznych ze zbioru "Adult Census", uwzględniających m.in. wiek, wykształcenie, zawód czy status rodzinny.

Projekt obejmuje pełny pipeline ML: od czyszczenia danych (EDA), przez inżynierię cech, aż po trening i ewaluację wielu modeli.

## Technologie i Biblioteki
Projekt został zrealizowany w języku Python z wykorzystaniem:
* **Pandas & NumPy** – manipulacja i analiza danych.
* **Scikit-learn** – budowa i trenowanie modeli, preprocessing.
* **Matplotlib & Seaborn** – wizualizacja danych i wyników (krzywe ROC, macierze pomyłek).

## Wyniki i Wnioski
W ramach eksperymentu przetestowano i porównano kilka algorytmów klasyfikacyjnych. Kluczowe wnioski:

1.  **Zwycięski model:** Najlepsze rezultaty osiągnął **Gradient Boosting**.
    * **Dokładność (Accuracy):** 86.6%
    * **F1-Score:** 0.719
2.  **Random Forest:** Zajął drugie miejsce. Charakteryzował się wysokim współczynnikiem *Recall* (dobrze wykrywał osoby zamożne), ale generował więcej fałszywych alarmów (False Positives) w porównaniu do Gradient Boostingu.
3.  **Ogólna wydajność:** Wszystkie testowane modele uzyskały zbliżone i wysokie wartości AUC, co potwierdza poprawność przeprowadzonego procesu inżynierii cech.

## 🚀 Jak uruchomić
1.  Sklonuj repozytorium:
    ```bash
    git clone [https://github.com/twoj-nick/adult-income-prediction.git](https://github.com/twoj-nick/adult-income-prediction.git)
    ```
2.  Zainstaluj wymagane biblioteki:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn
    ```
3.  Uruchom notebook w Jupyter Lab/Notebook lub VS Code:
    ```bash
    jupyter notebook ADULTS_income_prediction.ipynb
    ```

---
Autor: Ignacy Sieraczyński