# Detekcia podvodov s využitím metód dátovej analytiky

Projekt vznikol ako súčasť **bakalárskej práce** zameranej na detekciu podvodov pri samoobslužných pokladniach pomocou metód dátovej analytiky. Celý proces bol spracovaný v prostredí **Visual Studio Code** s využitím jupyter notebookov.

---
>### Abstrakt bakalárskej práce
>Práca sa zaoberá problematikou detekcie podvodného správania pri samoobslužných pokladniach v maloobchode, ktoré predstavujú moderný spôsob automatizácie nákupu. Vzhľadom na rastúci trend ich používania a súčasne  zvyšujúci sa výskyt bezpečnostných incidentov je cieľom práce identifikovať charakteristické znaky podvodov a vyhodnotiť možnosti ich automatickej detekcie pomocou modelov strojového učenia. Práca je spracovaná podľa metodiky CRISP-DM . Na spracovanie problému boli využité algoritmy Logistickej regresie, Naivného Bayesa, Náhodných lesov a LightGBM. S cieľom zvýšiť kvalitu vstupných údajov sme vykonali analýzu a transformáciu dát rôznymi spôsobmi. Zamerali sme sa aj na nevyváženosť cieľovej triedy pomocou metódy nadvzorkovania. Výkonnosť modelov sme porovnali na základe metrík ako presnosť, návratnosť, F1-skóre, úspešnosť a špecificita. Výsledky ukázali, že kvalitná príprava dát má výrazný vplyv na výkonnosť modelov. Najlepšie výsledky dosiahol model Náhodné Lesy na normalizovaných dátach. Na základe analýzy boli identifikované správania typické pre podvod, ktoré možno využiť pri návrhu systémov na automatizovanú prevenciu podvodov v praxi.
---
### Obsah repozitára
nt504wm/
├── Modelovanie/ 
│   ├── `LR.ipynb` – Logistická regresia  
│   ├── `LightGBM.ipynb` – Model LightGBM  
│   ├── `NB.ipynb` – Naívny Bayes
│   └── `RF.ipynb` – Náhodný les  
├── Pochopenie_dat/
│   ├── `Pochopenie_dat.ipynb` – Základná analýza a vizualizácia vstupných dát
│   ├── `fraud_test.csv` – Doplnkový súbor obsahujúci cieľový atribút k súboru `test.csv`  
│   ├── `test.csv` – Testovacie dáta bez klasifikácie (bez atribútu `fraud`)  
│   └── `train.csv` – Tréningové dáta s označením, či ide o podvod alebo nie 
├── Priprava_dat/
│   ├── `Priprava_dat.ipynb` – Úprava dát pre modelovanie
│   ├── `data.csv` – Spojené dáta z `train.csv`, `test.csv` a `fraud_test.csv`  
│   ├── `dis.csv` – Diskretizované dáta  
│   ├── `dis_red.csv` – Redukované diskretizované dáta  
│   ├── `fraud_test.csv` – Doplnkový súbor obsahujúci cieľový atribút k súboru `test.csv` 
│   ├── `norm.csv` – Normalizované dáta  
│   ├── `norm_red.csv` – Redukované normalizované dáta  
│   ├── `origin.csv` – Pôvodné, neupravené dáta  
│   ├── `origin_red.csv` – Redukované originálne dáta  
│   ├── `test.csv` – Testovacie dáta bez klasifikácie (bez atribútu `fraud`)  
│   └── `train.csv` – Tréningové dáta s označením, či ide o podvod alebo nie 
└── README.md

## Požiadavky
Dáta boli spracované v prostredí Visual Studio Code, notebooky sú vo formáte `.ipynb` a je ich možné otvoriť cez Jupyter Notebook alebo VS Code s rozšírením Python/Jupyter.

 - Python 3.12.4
 - imbalanced_learn 0.12.3 
 - lightgbm 4.6.0 
 - matplotlib 3.8.4
 - numpy 2.2.6 
 - pandas 2.2.3 
 - scikit_learn 1.4.2 
 - seaborn 0.13.2
### Príkaz na inštaláciu:
Na spustenie notebookov je potrebné mať nainštalované nasledovné knižnice. Projekt bol testovaný s **Python verziou 3.12.4**.

```bash
pip install imbalanced-learn==0.12.3 lightgbm==4.6.0 matplotlib==3.8.4 numpy==2.2.6 pandas==2.2.3 scikit-learn==1.4.2 seaborn==0.13.2
```  

---

### Autor - Natália Tomková

