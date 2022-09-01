# Econometrics Cheat Sheet

Econometrics cheat sheet created using $\LaTeX$ with a summarized review of:

* **Basic econometrics concepts**: econometrics definitions, data type, phases of a model, regression and correlation analysis.
* **Assumptions and properties** of the linear regression model.
* **Ordinary Least Squares** (OLS) equations, coefficient interpretatation, error measures, r-squared.
* **Hypothesis testing and confidence intervals**.
* **Dummy variables and structural change**.
* **Predictions**.
* **Popular OLS problems** (multicollinearity, heteroscedasticity and auto-correlation): consequences, detection and correction.

:bulb: Opinions, ideas and collaboration proposals are heard through GitHub or by email (marcelomijas@gmail.com). Also, my [LinkedIn](https://www.linkedin.com/in/marcelomorenop/).

### Download links

**Econometrics Cheat Sheet**. Current version: `2.3` (last updated 2 sep. 2022)

|         | PDF file                                                          | TeX file                                                            |
| :-----: | :---------------------------------------------------------------: | :-----------------------------------------------------------------: |
| English | [en.pdf](econometrics-cheatsheet/econometrics-cheatsheet-en.pdf)  | [en.tex](econometrics-cheatsheet/econometrics-cheatsheet-en.tex)    |
| Spanish | [es.pdf](econometrics-cheatsheet/econometrics-cheatsheet-es.pdf)  | [es.tex](econometrics-cheatsheet/econometrics-cheatsheet-es.tex)    |

## Roadmap

- [x] Release of pages 1 and 2 of `econometrics-cheatsheet` covering basic concepts, assumptions and properties, OLS equations, and more. Version `1.0`

- [x] Release of page 3 of `econometrics-cheatsheet` covering popular OLS problems. Version `2.0`

- [x] Release of an Spanish version of `econometrics-cheatsheet`.

- [ ] Release of a cheat cheet exclusively dedicated to time series in the context of econometrics (`time-series-cheatsheet`).

     :warning: A work in progress preview can be found [here](time-series-cheatsheet/time-series-cheatsheet-en.pdf), feedback is welcome.

- [ ] Release of an Spanish version of `time-series-cheatsheet`.

- [ ] Expansion and restructuring of the Econometrics Cheat Sheet Project in three documents: one introductory and concise summary of basic econometrics (Econometrics Cheat Sheet), one dedicated to the most common problems in econometrics (Econometrics Problems Cheat Sheet) and one dedicated to time series in econometrics (Time Series Cheat Sheet). The max lenght of each one will be two pages.

:question: Syled version of the cheat sheets (background colors, styled sections, more appealing plots, etc.)

## Frequently Asked Questions

### What does $residualized$ $x_j$ means?

Those are the residuals from a OLS regression between $x_j$ and all the other $x$ 's. Error measures and r-squared can also be obtained from this regression.

### Where is the non matrix version of the standard error of the $\hat{\beta}$ 's?

For space reasons, the version included in the cheatsheet is the matricial one. It is perfectly valid and equal to the non matrix version.

The non matrix version:

$$se(\hat{\beta}_j)=\sqrt{\frac{\hat{\sigma}^2}{SST_j(1-R^2_j)}},j=1,...,k$$

## Resources

In addition to the notes taken from the [Degree in Economics by the King Juan Carlos University](https://www.urjc.es/universidad/calidad/560-economia) and the [Master in Applied Statistics by Máxima Formación and Nebrija University](https://www.maximaformacion.es/masters/master-de-estadistica-aplicada-con-r-software/), the books used:

[1] Baltagi, B. H. (2011). *Econometrics*. New York: springer.

[2] Gujarati, D. N., Porter, D. C., & Gunasekar, S. (2012). *Basic econometrics*. Tata McGraw-Hill Education.

[3] James, G., Witten, D., Hastie, T., & Tibshirani, R. (2013). *An introduction to statistical learning*. New York: springer.

[4] Ruiz-Maya, L., & Pliego, F. J. M. (2004). *Fundamentos de inferencia estadística*. AC.

[5] Stock, J. H., & Watson, M. W. (2012). *Introduction to econometrics*. New York: Pearson.

[6] Wooldridge, J. M. (2015). *Introductory econometrics: A modern approach*. Cengage learning.

[7] Lütkepohl, H., & Krätzig, M. (Eds.). (2004). *Applied Time Series Econometrics*. Cambridge: Cambridge University Press.

## Contributions

* Reddit user \_bheg_ - Pointed out about the importance of including strong and weak exogeneity and their consequences on bias and consistency properties of OLS.

## Support my work

* SOL address: `Enj2bTkHoat79MWJ8rYrkvvX3GEPHKA98WME2yW3ff2`
* ETH address: `0x5Bc6287973D39EDfa4Da65Ec924CD7853791bD93`
