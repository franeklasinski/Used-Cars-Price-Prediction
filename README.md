# Used Car Price Prediction

Analiza i predykcja cen samochodów używanych przy użyciu uczenia maszynowego w Jupyter Notebook.

## Co zostało zrobione

### 1. **Eksploracyjna Analiza Danych (EDA)**
- Analiza podstawowych informacji o danych (kształt, typy, braki)
- Wizualizacje: histogram cen, boxplot, macierz korelacji, wykres gęstości
- Statystyki opisowe dla kolumn numerycznych
- Analiza cech kategorycznych i porównanie zbiorów train/test

### 2. **Preprocessing Danych**
- Czyszczenie danych (usunięcie braków i niepotrzebnych kolumn)
- One-Hot Encoding dla zmiennych kategorycznych
- StandardScaler dla zmiennych numerycznych
- Pipeline transformacji z ColumnTransformer

### 3. **Modelowanie ML**
- Porównanie 4 algorytmów: Linear/Ridge Regression, Random Forest, Gradient Boosting
- Ewaluacja na podstawie R², MAE, RMSE + czas trenowania
- Automatyczny wybór najlepszego modelu

### 4. **Wizualizacje Wyników**
- Porównanie metryk wszystkich modeli

## Technologie
- **Python** + Jupyter Notebook
- **Pandas, NumPy** - analiza danych
- **Matplotlib, Seaborn** - wizualizacje
- **Scikit-learn** - modele ML

## Uruchomienie
```bash
git clone https://github.com/franeklasinski/Used-Cars-Price-Prediction
.git
cd Used-Cars-Price-Prediction
jupyter notebook car-price.ipynb
```

### Porównane modele:
1. **Linear Regression** - baseline
2. **Ridge Regression** - z regularyzacją L2
3. **Random Forest** - ensemble drzew
4. **Gradient Boosting** - boosting

## Wyniki
```
Najlepszy model: Random Forest
R² Score: 0.8323
MAE: 1.74 
RMSE: 4.94  
```

## Struktura
```
predict-car-price/
├── car-price.ipynb     # Główny notebook
├── train-data.csv      # Dane treningowe
├── test-data.csv       # Dane testowe
└── README.md          # Dokumentacja
```

---

**Autor:** Franciszek Łasiński 
[@franeklasinski](https://github.com/franeklasinski)

*Projekt ML do predykcji cen samochodów - kompletny pipeline od EDA po wizualizacje wyników* 
