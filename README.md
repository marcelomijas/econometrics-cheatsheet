# Econometrics Cheat Sheet

Econometrics cheat sheet created using LaTeX with a summarized review of:

* **Basic econometrics concepts**: econometrics definitions, data type, phases of a model, regression and correlation analysis.
* **Assumptions and properties** of the linear regression model.
* **Ordinary Least Squares** (OLS) equations, coefficient interpretatation, error measures, r-squared.
* **Hypothesis testing and confidence intervals**.
* **Dummy variables and structural change**.
* **Predictions**.
* **Popular OLS problems** (multicollinearity, heteroscedasticity and auto-correlation): consequences, detection and correction.

### Download links

**Econometrics Cheat Sheet**. Current version: `2.2`

|         | PDF file | TeX file |
|---------|----------|----------|
| English |  [en.pdf](econometrics-cheatsheet/econometrics-cheatsheet-en.pdf)  |  [en.tex](econometrics-cheatsheet/econometrics-cheatsheet-en.tex)  |
| Spanish |  [es.pdf](econometrics-cheatsheet/econometrics-cheatsheet-es.pdf)  |  [es.tex](econometrics-cheatsheet/econometrics-cheatsheet-es.tex)  |


Opinions, ideas and collaboration proposals are heard through GitHub or by email (marcelomijas@gmail.com). Also, my [LinkedIn](https://www.linkedin.com/in/marcelomorenop/).

## Roadmap

:white_check_mark: Release of page 3 of econometrics-cheatsheet whith popular OLS problems.

:white_check_mark: Release of an Spanish version of the econometrics-cheatsheet.

:construction: Release of a cheat cheet exclusively dedicated to time series in the context of econometrics (time-series-cheatsheet). A preview of the Work In Progress can be seen [here](time-series-cheatsheet/time-series-cheatsheet-en.pdf), feedback is welcome.

## Frequently Asked Questions

### What does ![](https://render.githubusercontent.com/render/math?math=\text{residualized}x_j) means?

Those are the residuals from a OLS regression between ![](https://render.githubusercontent.com/render/math?math=x_j) and all the other ![](https://render.githubusercontent.com/render/math?math=x)'s. Error measures and r-squared can be obtained from this regression.

### Where is the non matrix version of the standard error of the ![](https://render.githubusercontent.com/render/math?math=\hat{\beta})'s?

For space reasons, the version included in the cheatsheet is the matricial one. It is perfectly valid and equal to the non matrix version.

The non matrix version:

![](https://render.githubusercontent.com/render/math?math=se(\hat{\beta}_j)=\sqrt{\frac{\hat{\sigma}^2}{SST_j(1-R^2_j)}},j=1,...,k)

## Bibliography

In addition to the notes taken from the [Degree in Economics by the King Juan Carlos University](https://www.urjc.es/universidad/calidad/560-economia) and the [Master in Applied Statistics by Máxima Formación with Nebrija University](https://www.maximaformacion.es/masters/master-de-estadistica-aplicada-con-r-software/), the books used:

[1] Baltagi, B. H. (2011). *Econometrics*. New York: springer.

[2] Gujarati, D. N., Porter, D. C., & Gunasekar, S. (2012). *Basic econometrics*. Tata McGraw-Hill Education.

[3] James, G., Witten, D., Hastie, T., & Tibshirani, R. (2013). *An introduction to statistical learning*. New York: springer.

[4] Ruiz-Maya, L., & Pliego, F. J. M. (2004). *Fundamentos de inferencia estadística*. AC.

[5] Stock, J. H., & Watson, M. W. (2012). *Introduction to econometrics*. New York: Pearson.

[6] Wooldridge, J. M. (2015). *Introductory econometrics: A modern approach*. Cengage learning.

## Contributions

* Reddit user \_bheg_ - Pointed out about the importance of including strong and weak exogeneity and their consequences on bias and consistency properties of OLS.
