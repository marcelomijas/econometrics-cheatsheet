# The Econometrics Cheat Sheet Project

Econometrics cheat sheets created using $\LaTeX$:

* **Econometrics Cheat Sheet**: Basic econometrics concepts, OLS assumptions, properties, interpretation, error measuremets, hypothesis testing, confidence intervals, dummy variables, structural change, summary of popular OLS problems and more!
* **Time Series Cheat Sheet**: Components of a time series, seasonality, auto-correlation, stationarity, weak and strong dependence, cointegration and heterocedasticity on time series.
* **Additional Cheat Sheet**: Matrix notation of OLS, variable omission, proxy variables, instrumental variables, TSLS, information criterias, non-restricted hypothesis test, incorrect functional form, logistic regression, statistical definitions, VAR models and VECM.

:bulb: I am currently pursuing a PhD in macroeconomics and econometrics at Universidad Rey Juan Carlos (Madrid, Spain). Also, I am a [researcher and professor](https://gestion2.urjc.es/pdi/ver/marcelo.moreno) at the same institution. Collaboration proposals and academic stays offers in other universities (national and international) are welcome and can help me a lot in my career! :rocket:

:triangular_flag_on_post: [LinkedIn](https://www.linkedin.com/in/marcelomorenop/). Please, send me a message when connecting or I will ignore the request.

:globe_with_meridians: Do you want to translate any of these cheat sheets to your language? Open an issue and I will provide instructions.

:printer: If you want to print them two-sided, select the *Flip on Short Edge* option on your printer.

## Download links

| Econometrics | PDF | TeX |
| :---: | :---: | :---: |
| English :uk: | [`CS-24.5.2`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/econometrics-cheatsheet/econometrics-cheatsheet-en.pdf) | [`CS-24.5.2`](econometrics-cheatsheet/econometrics-cheatsheet-en.tex)
| Spanish :es: | [`CS-24.5.2`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/econometrics-cheatsheet/econometrics-cheatsheet-es.pdf) | [`CS-24.5.2`](econometrics-cheatsheet/econometrics-cheatsheet-es.tex)

| Time Series | PDF | TeX |
| :---: | :---: | :---: |
| English :uk: | [`TS-24.8.1`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/time-series-cheatsheet/time-series-cheatsheet-en.pdf) | [`TS-24.8.1`](time-series-cheatsheet/time-series-cheatsheet-en.tex)
| Spanish :es: | [`TS-24.8.1`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/time-series-cheatsheet/time-series-cheatsheet-es.pdf) | [`TS-24.8.1`](time-series-cheatsheet/time-series-cheatsheet-es.tex)

| Additional | PDF | TeX |
| :---: | :---: | :---: |
| English :uk: | [`ADD-24.6`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/additional-cheatsheet/additional-cheatsheet-en.pdf) | [`ADD-24.6`](additional-cheatsheet/additional-cheatsheet-en.tex)
| Spanish :es: | [`ADD-24.6`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/additional-cheatsheet/additional-cheatsheet-es.pdf) | [`ADD-24.6`](additional-cheatsheet/additional-cheatsheet-es.tex)

Complete set (PDF and TeX, all languages): [ZIP](https://github.com/marcelomijas/econometrics-cheatsheet/archive/refs/heads/main.zip)

## Frequently Asked Questions (FAQ)

### What does $\mathrm{resid}$ $x_j$ mean?

Those are the residuals from a OLS regression between $x_j$ and all the other $x$ 's.

### Why is $\beta_0$ the constant term? My reference manual / professor's definition of the econometric model is different.

There is some debate about the correct way to name the coefficients, their sub-index and the sub-index of the variables of a model. The naming could have an impact on how some statistics like the adjusted R-squared or some tests like the F test are written.

For example, while some econometricians write the multiple regression model with a constant term like this:

$$y_i = \beta_0 + \beta_1 x_{1i} + ... + \beta_k x_{ki} + u_i \quad (1)$$

There are others that refer to that same econometric model as:

$$y_i = \beta_1 + \beta_2 x_{2i} + ... + \beta_k x_{Ki} + u_i \quad (2)$$

And others refer as:

$$y_i = \alpha + \beta_1 x_{1i} + ... + \beta_k x_{ki} + u_i \quad (3)$$

All the above are equally valid representations of the multiple regression model. In the specification $(1)$, $\beta_0$ represents the constant term, while in specifications $(2)$ and $(3)$, it is represented by $\beta_1$ and $\alpha$, respectively.

In this project, the main specification used is the first $(1)$, so we can say that there are $k$ independent variables and $k + 1$ coefficients (including the constant term). The same could be said for the specification $(3)$, that it is used punctually in the project. There are no differences in the statistics and tests formula definition between specifications $(1)$ and $(3)$.

The specification $(2)$, is different from the rest, since $K \neq k$. In this specification, it could be said that there are $K - 1$ independent variables and $K$ coefficients (including the constant term).

For specification $(2)$ users, not everything is lost. There is a relation between these three specifications: $K = k + 1$, so $k = K - 1$. This way, a "translation" between formulas for different representations is possible (by the user). For example, the adjusted R-squared:

$$(1, 3) \quad \overline{R}^2 = 1 - \frac{n - 1}{n - k - 1} \cdot (1 - R^2)$$

$$(2) \quad \overline{R}^2 = 1 - \frac{n - 1}{n - (K - 1) - 1} \cdot (1 - R^2) =$$

$$= 1 - \frac{n - 1}{n - K} \cdot (1 - R^2)$$

### Where is the non matrix version of the standard error of the $\hat{\beta}$ 's?

For space reasons, the version included in the cheatsheet is the matricial one. It is perfectly valid and equal to the non matrix version.

The non matrix version:

$$\mathrm{se}(\hat{\beta}_j)=\sqrt{\frac{\hat{\sigma}^2_u}{\mathrm{SST}_j \cdot (1-R^2_j)}} \quad , \quad j=1,...,k$$

### Why don't they have 2 or 4 pages each?

Each of them are 3 pages long, and there are no plans on changing that for the time being.

I understand that if you print them two-sided, the second page ends up with an empty side. Consider this as an space to take your own notes :smile:.

Currently, I am very comfortable with the content and font size used. Also, all cheat cheets are made in a way that you can combine any page of one with any page of another or skip them.

## Resources

In addition to the notes taken from the [Degree in Economics](https://www.urjc.es/universidad/calidad/560-economia) and [Master in Modern Economic Analysis](https://www.urjc.es/estudios/master/786-analisis-economico-moderno) by Universidad Rey Juan Carlos, and the [Master in Applied Statistics](https://www.maximaformacion.es/masters/master-de-estadistica-aplicada-con-r-software/) by Máxima Formación and Universidad Nebrija, the books used:

[1] Baltagi, B. H. (2011). *Econometrics*. New York: Springer.

[2] Gujarati, D. N., Porter, D. C., & Gunasekar, S. (2012). *Basic econometrics*. Tata McGraw-Hill Education.

[3] James, G., Witten, D., Hastie, T., & Tibshirani, R. (2013). *An introduction to statistical learning*. New York: Springer.

[4] Lütkepohl, H., & Krätzig, M. (Eds.). (2004). *Applied Time Series Econometrics*. Cambridge: Cambridge University Press.

[5] Pfaff, B. (2011). *Analysis of integrated and cointegrated time series with R*. New York: Springer.

[6] Ruiz-Maya, L., & Pliego, F. J. M. (2004). *Fundamentos de inferencia estadística*. AC.

[7] Stock, J. H., & Watson, M. W. (2012). *Introduction to econometrics*. New York: Pearson.

[8] Wooldridge, J. M. (2015). *Introductory econometrics: A modern approach*. Cengage learning.

## Contributions

* Reddit user \_bheg_ - Pointed out about the importance of including strong and weak exogeneity and their consequences on bias and consistency properties of OLS.

## Support the project

The first way to help the project is to **directly support the authors of the manuals that are included in the resources section** (for example, by buying their works). Each and every one of the authors of the manuals are wonderful minds who have contributed a lot to econometrics and statistics. Another great way to support the project is by sharing it and :star: it!
