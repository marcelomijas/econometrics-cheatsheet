# The Econometrics Cheat Sheet Project

Econometrics cheat sheets created using $\LaTeX$:

* **Econometrics Cheat Sheet**: Basic econometrics concepts, OLS assumptions and properties, coefficient interpretatation, error measures, R-squared, hypothesis testing and confidence intervals, dummy variables and structural change, summary of popular OLS problems and more!.
* **Time Series Cheat Sheet**: Components of a time series, trends and seasonality, auto-correlation, stationarity, weak and strong dependence, cointegration and heterocedasticity on time series.
* **Additional Cheat Sheet**: Matrix notation of OLS, variable omission problem, proxy variables, instrumental variables, Two Stage Least Squares, information criteria, non-restricted hypothesis test, incorrect functional form, logistic regression, statistical definitions, VAR models, VECM.

:bulb: I am currently doing my PhD in macroeconomics and econometrics at King Juan Carlos University (Madrid, Spain). Also, I am a researcher and professor at the same institution. Collaboration proposals and academic stays offers in other universities (national and international) are considered and can help me a lot in my career!

My [LinkedIn](https://www.linkedin.com/in/marcelomorenop/) (please, send me a message when "connect" or I will ignore the request).

### Download links

**Econometrics Cheat Sheet**. Current version: `3.2` (last updated Jun. 22, 2023)

|              | PDF file                                                          | TeX file                                                          |
| :----------: | :---------------------------------------------------------------: | :---------------------------------------------------------------: |
| English :uk: | [en.pdf](econometrics-cheatsheet/econometrics-cheatsheet-en.pdf)  | [en.tex](econometrics-cheatsheet/econometrics-cheatsheet-en.tex)  |
| Spanish :es: | [es.pdf](econometrics-cheatsheet/econometrics-cheatsheet-es.pdf)  | [es.tex](econometrics-cheatsheet/econometrics-cheatsheet-es.tex)  |

**Time Series Cheat Sheet**. Current version: `ts1.9` (last updated Jun. 22, 2023)

|              | PDF file                                                        | TeX file                                                        |
| :----------: | :-------------------------------------------------------------: | :-------------------------------------------------------------: |
| English :uk: | [en.pdf](time-series-cheatsheet/time-series-cheatsheet-en.pdf)  | [en.tex](time-series-cheatsheet/time-series-cheatsheet-en.tex)  |
| Spanish :es: | [es.pdf](time-series-cheatsheet/time-series-cheatsheet-es.pdf)  | [es.tex](time-series-cheatsheet/time-series-cheatsheet-es.tex)  |


**Additional Cheat Sheet**. Current version: `add1.4` (last updated Jun. 22, 2023)

|              | PDF file                                                      | TeX file                                                      |
| :----------: | :-----------------------------------------------------------: | :-----------------------------------------------------------: |
| English :uk: | [en.pdf](additional-cheatsheet/additional-cheatsheet-en.pdf)  | [en.tex](additional-cheatsheet/additional-cheatsheet-en.tex)  |
| Spanish :es: | [es.pdf](additional-cheatsheet/additional-cheatsheet-es.pdf)  | [es.tex](additional-cheatsheet/additional-cheatsheet-es.tex)  |

## Frequently Asked Questions (FAQ)

### What does $\mathrm{resid}$ $x_j$ mean?

Those are the residuals from a OLS regression between $x_j$ and all the other $x$ 's. Error measures and R-squared can also be obtained from this regression.

### Why is $\beta_0$ the constant term? My reference manual / professor's definition of the econometric model is different.

There is some debate about the correct way to name the coefficients, their sub-index and the sub-index of the variables of a model. The naming could have an impact on how some statistics like the adjusted R-squared or some tests like the F test are written.

For example, while some econometricians write the multiple regression model with a constant term like this:

$$y_i = \beta_0 + \beta_1 x_{1i} + ... + \beta_k x_{ki} + u_i \rightarrow (1)$$

There are others that refer to that same econometric model as:

$$y_i = \beta_1 + \beta_2 x_{2i} + ... + \beta_k x_{Ki} + u_i \rightarrow (2)$$

And others refer as:

$$y_i = \alpha + \beta_1 x_{1i} + ... + \beta_k x_{ki} + u_i \rightarrow (3)$$

All the above are equally valid representations of the multiple regression model. In the specification $(1)$, $\beta_0$ represents the constant term, while in specifications $(2)$ and $(3)$, it is represented by $\beta_1$ and $\alpha$, respectively.

In this project, the main specification used is the first $(1)$, so we can say that there are $k$ independent variables and $k + 1$ coefficients (including the constant term). The same could be said for the specification $(3)$, that it is used punctually in the project. There are no differences in the statistics and tests formula definition between specifications $(1)$ and $(3)$.

The specification $(2)$, is different from the rest, since $K \neq k$. In this specification, it could be said that there are $K - 1$ independent variables and $K$ coefficients (including the constant term).

For specification $(2)$ users, not everything is lost. There is a relation between these three specifications: $K = (k + 1)$, so $k = (K - 1)$. This way, a "translation" between formulas for different representations is possible (by the user). For example, the adjusted R-squared:

$$(1)(3) \rightarrow \overline{R}^2 = 1 - \frac{n - 1}{n - k - 1} \cdot (1 - R^2)$$

$$(2) \rightarrow \overline{R}^2 = 1 - \frac{n - 1}{n - (K - 1) - 1} \cdot (1 - R^2) =$$

$$= 1 - \frac{n - 1}{n - K} \cdot (1 - R^2)$$

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
