# Wybrane metody identyfikacji obserwacji odstających w szeregach czasowych
### Autor: Piotr Migdałek
#### Promotor: dr inż. Adam Zagdański

#### Opis pracy:
Praca przedstawia wybrane techniki detekcji oraz modelowania obserwacji odstających w szeregach czasowych. Jej istotą jest wykorzystanie narzędzi statystycznych oraz algorytmów do analizy realnych problemów, z którymi zmagają się na co dzień specjaliści z różnych dziedzin nauki, przemysłu i biznesu. Struktura pracy obejmuje niezbędne wprowadzenie teoretyczne oraz kolejne rozdziały, w których skupiono się na na konkretnych postaciach anomalii: interwencjach, punktowych obserwacjach odstających oraz sekwencjach.

# Selected outlier detection methods in time series data
### Author: Piotr Migdałek
#### Supervisor: dr inż. Adam Zagdański

#### Brief description:
The thesis discusses selected outlier detection methods in time series data. The core of presented work consists of practical analysis of real-world problems from different fields of science, industry and business using statistical and algorithmic approaches. The thesis comprises of necessary theoretical background followed by chapters covering particular types of anomalies: interventions, point outliers and sequences.

## Repo contents
Compiled LaTeX file with thesis can be viewied via outliers_thesis.pdf. It includes all theory and studies and research results with documentation carried out in R package.

First chapter consists of basic theory concerning time series, autocorrelation, ARIMA modelling, useful statistical tests and time series decomposition techniques. All graphical examples were prepared by me using ggplot2, forecast and patchwork libraries.

Second chapter is focused on parametrizing various outliers effect in order to detect them and incorporate to regression models with ARIMA errors. I prepared vast forecasting analysis of CO2 emission in Poland -- using mainly ARIMAX, ARIMA and ETS models also prepared solely in R with help of forecast, tsoutliers and ggplot2 libraries. 

Third chapter introduces numerous point outlier detection techniques in univariate streaming data. 

Fourth chapter has a little bit pattern mining twist to it, because it extends outliers taxonomy to sequences. I introduce simple brute force approach, its heuristic modification HOT-SAX as well as whole new data mining structure -- Matrix Profile. 

