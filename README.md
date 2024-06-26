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
* Files in this repo contain all theory, studies, research, documentation and results carried out in <tt>R</tt> package.
  * *outliers_thesis.pdf* – compiled thesis written in LaTeX (in Polish)
  * *outliers_presentation.pdf* – presentation of most significant topics/results concerning presented work

* First chapter consists of basic theory concerning time series, autocorrelation, ARIMA modelling, useful statistical tests and time series decomposition techniques. All graphical examples were prepared by me using <tt>ggplot2</tt>, <tt>forecast</tt> and <tt>patchwork</tt> libraries.

* Second chapter is focused on parametrizing various outlier effects using intervention models in order to detect and incorporate them into regression model with ARIMA errors. I prepared vast **forecasting analysis of CO2 emission in Poland** – using mainly ARIMAX, ARIMA and ETS models also prepared solely in <tt>R</tt> with help of <tt>forecast</tt>, <tt>tsoutliers</tt> and <tt>ggplot2</tt> libraries.

<div style="text-align: center;">
<img width="850" alt="lic_1" src="https://github.com/piotrmigdalek/time-series-outliers-thesis/assets/101133937/3edcca23-7231-4ab2-846a-3f96ea1bd1bd">
</div>

* Third chapter introduces numerous **point outlier detection techniques in univariate streaming data**. I made comparison of different detection methods implemented in various <tt>R</tt> libraries and also designed my own methods. I used:

Algorithm | Description | Implementation
------------- | ------------- | -------------
<tt>tso</tt> | Chen and Liu iterative procedure of simultaneous parameter estimation and outlier detection | <tt>tsoutliers</tt>
<tt>locate.outliers</tt>  | Statistical test based on ARIMA residuals | <tt>tsoutliers</tt>
<tt>tsoutliers</tt>  | STL decomposition + Tukey box plot rule for far out values | <tt>forecast</tt>
<tt>OSWM</tt>  | STL decomposition + one-sided moving average/median thresholding | mine
<tt>TSWM</tt>  | STL decomposition + two-sided moving average/median thresholding | mine
<tt>detect_outliers</tt>  | STL decomposition + GMM + clustering | <tt>tsrobprep</tt>
<tt>ad_vec</tt> | Modified STL decomposition + Rosner test | <tt>AnomalyDetection</tt>


* Fourth chapter has a little bit of a pattern mining twist to it, because it extends outliers taxonomy to sequences. I discussed simple brute force approach, its heuristic modification HOT-SAX as well as whole recently introduced data mining structure – Matrix Profile. These approaches are evaluated in **anomalous heartbeat detection in ECG data** case study using mainly <tt>R</tt> libraries <tt>jmotif</tt> and <tt>tsmp</tt>.

<div style="text-align: center;">
<img width="850" alt="lic2" src="https://github.com/piotrmigdalek/time-series-outliers-thesis/assets/101133937/cdb3b28f-660a-4db4-a948-6faa2c6bea2d">
</div>
