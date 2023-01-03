# Econometrics Cheat Sheet Project

Econometrics cheat sheets created using $\LaTeX$ with a summarized review of:

* **Econometrics Cheat Sheet**: Basic econometrics concepts (econometrics definitions, data types, phases of a model, regression and correlation analysis), OLS assumptions and properties, equations, coefficient interpretatation, error measures, R-squared, hypothesis testing and confidence intervals, dummy variables and structural change, predictions basics and summary of popular OLS problems (multicollinearity, heteroscedasticity and auto-correlation): consequences, detection and correction.
* **Time Series Cheat Sheet**: components of a time series, trends and seasonality, auto-correlation, stationarity, weak and strong dependence, cointegration and heterocedasticity on time series.
* **Additional Cheat Sheet**: matrix notation of OLS (estimation, variance-covariance of the betas and residuals, error measures), variable omission problem, proxy variables, instrumental variables, Two Stage Least Squares, information criteria, incorrect functional form, VAR models, VECM.

:bulb: Opinions, ideas and collaboration proposals are heard through GitHub or by email (marcelomijas@gmail.com). Also, my [LinkedIn](https://www.linkedin.com/in/marcelomorenop/) (please, send me a message before "connect" or I will ignore the request).

:mortar_board: I am currently doing my PhD in macroeconomics and econometrics at the King Juan Carlos University (Madrid, Spain). Article collaborations proposals and academic stays offers in other universities (national and international) are considered and can help me a lot in my career!

### Download links

**Econometrics Cheat Sheet**. Current version: `3.0` (last updated 3 jan. 2023)

|              | PDF file                                                          | TeX file                                                          |
| :----------: | :---------------------------------------------------------------: | :---------------------------------------------------------------: |
| English :uk: | [en.pdf](econometrics-cheatsheet/econometrics-cheatsheet-en.pdf)  | [en.tex](econometrics-cheatsheet/econometrics-cheatsheet-en.tex)  |
| Spanish :es: | [es.pdf](econometrics-cheatsheet/econometrics-cheatsheet-es.pdf)  | [es.tex](econometrics-cheatsheet/econometrics-cheatsheet-es.tex)  |

**Time Series Cheat Sheet**. Current version: `ts1.5` (last updated 3 jan. 2023)

|              | PDF file                                                        | TeX file                                                        |
| :----------: | :-------------------------------------------------------------: | :-------------------------------------------------------------: |
| English :uk: | [en.pdf](time-series-cheatsheet/time-series-cheatsheet-en.pdf)  | [en.tex](time-series-cheatsheet/time-series-cheatsheet-en.tex)  |
| Spanish :es: | [es.pdf](time-series-cheatsheet/time-series-cheatsheet-es.pdf)  | [es.tex](time-series-cheatsheet/time-series-cheatsheet-es.tex)  |


**Additional Cheat Sheet**. Current version: `add1.0` (last updated 3 jan. 2023)

|              | PDF file                                                        | TeX file                                                        |
| :----------: | :-------------------------------------------------------------: | :-------------------------------------------------------------: |
| English :uk: | [en.pdf](additional-cheatsheet/additional-cheatsheet-en.pdf)  | [en.tex](additional-cheatsheet/additional-cheatsheet-en.tex)  |
| Spanish :es: | [es.pdf](additional-cheatsheet/additional-cheatsheet-es.pdf)  | [es.tex](additional-cheatsheet/additional-cheatsheet-es.tex)  |

## Roadmap

- [x] Release of pages 1 and 2 of `econometrics-cheatsheet` covering basic concepts, assumptions and properties, OLS equations, and more.

- [x] Release of page 3 of `econometrics-cheatsheet` covering popular OLS problems.

- [x] Release of an Spanish version of `econometrics-cheatsheet`.

- [x] Release of a cheat sheet exclusively dedicated to time series in the context of econometrics, `time-series-cheatsheet`.

- [x] Release of an Spanish version of `time-series-cheatsheet`.

- [x] Release of a cheat sheet with more common problems in econometrics and additional models (VAR, VECM, ...), `additional-cheatsheet`.

- [ ] Styled version of the cheat sheets (background colors, styled sections, more appealing plots, etc.)

## Frequently Asked Questions (FAQ)

### What does $\mathrm{residualized}$ $x_j$ means?

Those are the residuals from a OLS regression between $x_j$ and all the other $x$ 's. Error measures and R-squared can also be obtained from this regression.

### Why is $\beta_0$ the constant term? My reference manual / professor's definition of the econometric model is different.

There is some debate about the correct way to name the coefficients, their sub-index and the sub-index of the variables of a model. The naming could have an impact on how some statistics like the adjusted R-squared or some tests like the F contrast formulas are written.

For example, while some econometricians write the multiple regression model with a constant term like this:

$$y_i = \beta_0 + \beta_1 x_{1i} + ... + \beta_k x_{ki} + u_i \rightarrow (1)$$

There are others that refer to that same econometric model as:

$$y_i = \beta_1 + \beta_2 x_{2i} + ... + \beta_k x_{ki} + u_i \rightarrow (2)$$

And others refer as:

$$y_i = \alpha + \beta_1 x_{1i} + ... + \beta_k x_{ki} + u_i \rightarrow (3)$$

All the above are equally valid representations of the multiple regression model. In the specification $(1)$, $\beta_0$ represents the constant term, while in specifications $(2)$ and $(3)$, it is represented by $\beta_1$ and $\alpha$, respectively.

In this project, the main specification used is the first $(1)$, so we can say that there are $k$ independent variables and $k+1$ coefficients (including the constant term), the same could be said for the specification $(3)$ (that it is used punctually). There are no differences in the statistics and tests formula definition between this two specifications, because $k_{(1)} = k_{(3)}$.

The specification $(2)$, is different from the rest: $k_{(1)} = k_{(3)} \neq k_{(2)}$. In this specification, it could be said that there are $k-1$ independent variables and $k$ coefficients (including the constant term).

For specification $(2)$ users, not everything is lost. There is a relation between the three specifications: $k_{(2)} = k_{(1)} + 1$, so $k_{(1)} = k_{(2)} - 1$, and also considering $k_{(1)} = k_{(3)}$. This way, a "translation" between formulas for different representations is possible (by the user). For example, the adjusted R-squared:

$$(1)(3) \rightarrow \overline{R}^2 = 1 - \frac{n-1}{n-k_{(1)}-1} \cdot (1-R^2)$$

$$(2) \rightarrow \overline{R}^2 = 1 - \frac{n-1}{n-(k_{(2)}-1)-1} \cdot (1-R^2) =$$

$$= 1 - \frac{n-1}{n-k_{(2)}} \cdot (1-R^2)$$

### Where is the non matrix version of the standard error of the $\hat{\beta}$ 's?

For space reasons, the version included in the cheatsheet is the matricial one. It is perfectly valid and equal to the non matrix version.

The non matrix version:

$$\mathrm{se}(\hat{\beta}_j)=\sqrt{\frac{\hat{\sigma}^2_u}{\mathrm{SST}_j \cdot (1-R^2_j)}} \quad , \quad j=1,...,k$$

## Resources

In addition to the notes taken from the [Degree in Economics by the King Juan Carlos University](https://www.urjc.es/universidad/calidad/560-economia) and the [Master in Applied Statistics by Máxima Formación and Nebrija University](https://www.maximaformacion.es/masters/master-de-estadistica-aplicada-con-r-software/), the books used:

[1] Baltagi, B. H. (2011). *Econometrics*. New York: springer.

[2] Gujarati, D. N., Porter, D. C., & Gunasekar, S. (2012). *Basic econometrics*. Tata McGraw-Hill Education.

[3] James, G., Witten, D., Hastie, T., & Tibshirani, R. (2013). *An introduction to statistical learning*. New York: springer.

[4] Lütkepohl, H., & Krätzig, M. (Eds.). (2004). *Applied Time Series Econometrics*. Cambridge: Cambridge University Press.

[5] Ruiz-Maya, L., & Pliego, F. J. M. (2004). *Fundamentos de inferencia estadística*. AC.

[6] Stock, J. H., & Watson, M. W. (2012). *Introduction to econometrics*. New York: Pearson.

[7] Wooldridge, J. M. (2015). *Introductory econometrics: A modern approach*. Cengage learning.

## Contributions

* Reddit user \_bheg_ - Pointed out about the importance of including strong and weak exogeneity and their consequences on bias and consistency properties of OLS.

## Support the project

The first (and I think, **the best**) way to help the project is to **directly support the authors of the manuals that are included in the resources section** (for example, by buying their works). Each and every one of the authors of the manuals are wonderful minds who have contributed a lot to econometrics and statistics. 

Another great way to support the project is by sharing it and :star: it!
