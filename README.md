﻿# The Econometrics Cheat Sheet Project

Econometrics cheat sheets created using $\LaTeX$:

* **Econometrics Cheat Sheet**: Basic concepts, OLS assumptions, properties, interpretation, error measurements, hypothesis testing, confidence intervals, dummy variables, structural change, popular problems, and more!
* **Time Series Cheat Sheet**: Series components, seasonality, autocorrelation, stationarity, cointegration and heterocedasticity on time series.
* **Additional Cheat Sheet**: OLS matrix notation, variable omission, proxy and instrumental variables, TSLS, information criteria, hypothesis testing (+), functional form, logistic regression, statistical definitions, VAR, SVAR, VECM.

:bulb: I am currently pursuing a PhD at Universidad Rey Juan Carlos (Madrid, Spain). Also, I am a [researcher and professor](https://gestion2.urjc.es/pdi/ver/marcelo.moreno) at the same institution. Collaboration proposals and academic stays offers in national/international universities are welcome! :rocket:

:triangular_flag_on_post: [LinkedIn](https://www.linkedin.com/in/marcelomorenop/). Please, send me a message when connecting, or I will ignore the request.

## Download links

| Econometrics | PDF | TeX |
| :---: | :---: | :---: |
| English :uk: | [`CS-25.01`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/econometrics-cheatsheet/econometrics-cheatsheet-en.pdf) | [`CS-25.01`](econometrics-cheatsheet/econometrics-cheatsheet-en.tex)
| Spanish :es: | [`CS-25.01`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/econometrics-cheatsheet/econometrics-cheatsheet-es.pdf) | [`CS-25.01`](econometrics-cheatsheet/econometrics-cheatsheet-es.tex)

| Time Series | PDF | TeX |
| :---: | :---: | :---: |
| English :uk: | [`TS-25.05`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/time-series-cheatsheet/time-series-cheatsheet-en.pdf) | [`TS-25.05`](time-series-cheatsheet/time-series-cheatsheet-en.tex)
| Spanish :es: | [`TS-25.05`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/time-series-cheatsheet/time-series-cheatsheet-es.pdf) | [`TS-25.05`](time-series-cheatsheet/time-series-cheatsheet-es.tex)

| Additional | PDF | TeX |
| :---: | :---: | :---: |
| English :uk: | [`ADD-25.05`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/additional-cheatsheet/additional-cheatsheet-en.pdf) | [`ADD-25.05`](additional-cheatsheet/additional-cheatsheet-en.tex)
| Spanish :es: | [`ADD-25.05`](https://raw.githubusercontent.com/marcelomijas/econometrics-cheatsheet/main/additional-cheatsheet/additional-cheatsheet-es.pdf) | [`ADD-25.05`](additional-cheatsheet/additional-cheatsheet-es.tex)

Complete set (PDF and TeX, all languages): [`ZIP`](https://github.com/marcelomijas/econometrics-cheatsheet/archive/refs/heads/main.zip)

:printer: If you want to print them two-sided, select the *Flip on Short Edge* option on your printer.

:globe_with_meridians: Do you want to translate any of these cheat sheets to your language? Open an issue and I will provide instructions.

:computer: Do you use R? Check out [*Applied Econometrics with R*](https://www.zeileis.org/teaching/AER/) by Christian Kleiber and Achim Zeileis!

## Frequently Asked Questions (FAQ)

### What does $\mathrm{resid}$ $x_j$ mean?

Those are the residuals from an OLS regression between $x_j$ and all the other $x$ 's.

### Why is $\beta_0$ the constant term? My reference manual/professor's definition of the econometric model is different.

There is some debate about the correct way to name the coefficients, their sub-index and the sub-index of the variables of a model. The naming could have an impact on how some statistics like the adjusted R-squared or some tests like the F test are written.

For example, while some econometricians write the multiple regression model with a constant term like this:

$$y_i = \beta_0 + \beta_1 x_{1i} + ... + \beta_k x_{ki} + u_i \quad (1)$$

Others refer to that same econometric model as:

$$y_i = \beta_1 + \beta_2 x_{2i} + ... + \beta_K x_{Ki} + u_i \quad (2)$$

And others refer to as:

$$y_i = \alpha + \beta_1 x_{1i} + ... + \beta_k x_{ki} + u_i \quad (3)$$

All the above are equally valid representations of the multiple regression model. In the specification $(1)$, $\beta_0$ represents the constant term, while in specifications $(2)$ and $(3)$, it is represented by $\beta_1$ and $\alpha$, respectively.

In this project, the main specification used is the first $(1)$, so we can say that there are $k$ independent variables and $k + 1$ coefficients (including the constant term). The same could be said for the specification $(3)$, that it is used punctually in the project. There are no differences in the statistics and tests formula definition between specifications $(1)$ and $(3)$.

The specification $(2)$ is different from the rest, since $K \neq k$. In this specification, it could be said that there are $K-1$ independent variables and $K$ coefficients (including the constant term).

For specification $(2)$ users, not everything is lost. There is a relation between these three specifications: $K = k + 1$, so $k = K - 1$. This way, a "translation" between formulas for different representations is possible (by the user). For example, the adjusted R-squared:

$$(1, 3) \quad \overline{R}^2 = 1 - \frac{n - 1}{n - k - 1} \cdot (1 - R^2)$$

$$(2) \quad \overline{R}^2 = 1 - \frac{n - 1}{n - (K - 1) - 1} \cdot (1 - R^2) =$$

$$= 1 - \frac{n - 1}{n - K} \cdot (1 - R^2)$$

### Where is the nonmatrix version of the standard error of the $\hat{\beta}$ 's?

For space reasons, the version included in the cheatsheet is the matrix one. It is perfectly valid and equal to the nonmatrix version.

The nonmatrix version:

$$\mathrm{se}(\hat{\beta}_j)=\sqrt{\frac{\hat{\sigma}^2_u}{\mathrm{SST}_j \cdot (1-R^2_j)}} \quad , \quad j=1,...,k$$

### Why don't they have 2 or 4 pages each?

Each of them are 3 pages long, and there are no plans on changing that for the time being.

I understand that if you print them two-sided, the second page ends up with an empty side. Consider this a space to take your notes.

Currently, I am very comfortable with the content and font size used. Also, all cheat cheets are made in a way that you can combine any page of one with any page of another or skip them.

## Resources

In addition to the notes taken from the [Degree in Economics](https://www.urjc.es/universidad/calidad/560-economia) and [Master in Modern Economic Analysis](https://www.urjc.es/estudios/master/786-analisis-economico-moderno) by Universidad Rey Juan Carlos, and the [Master in Applied Statistics](https://www.maximaformacion.es/masters/master-de-estadistica-aplicada-con-r-software/) by Máxima Formación and Universidad Nebrija, the books used are:

[1] Baltagi, B. H. (2011). *Econometrics*. New York: Springer.

[2] Gujarati, D. N., Porter, D. C., & Gunasekar, S. (2012). *Basic econometrics*. Tata McGraw-Hill Education.

[3] James, G., Witten, D., Hastie, T., & Tibshirani, R. (2013). *An introduction to statistical learning*. New York: Springer.

[4] Lütkepohl, H., & Krätzig, M. (Eds.). (2004). *Applied Time Series Econometrics*. Cambridge: Cambridge University Press.

[5] Oracle Crystal Ball Reference and Examples Guide. *Theil's U*. https://docs.oracle.com/cd/E57185_01/CBREG/ch06s02s03s04.html. Accessed May 18, 2025.

[6] Pfaff, B. (2011). *Analysis of integrated and cointegrated time series with R*. New York: Springer.

[7] Ruiz-Maya, L., & Pliego, F. J. M. (2004). *Fundamentos de inferencia estadística*. AC.

[8] Stock, J. H., & Watson, M. W. (2012). *Introduction to econometrics*. New York: Pearson.

[9] Tilburg Science Hub. *Panel Data*. https://tilburgsciencehub.com/topics/analyze/causal-inference/panel-data/#. Accessed May 18, 2025.

[10] Wooldridge, J. M. (2015). *Introductory econometrics: A modern approach*. Cengage learning.

## Contributions

* Reddit user \_bheg_ - Pointed out about the importance of including strong and weak exogeneity and their consequences on bias and consistency properties of OLS.

## Support the project

The first way to help the project is to **directly support the authors of the manuals that are included in the resources section** (for example, by buying their works). Every one of the authors of the manuals is a wonderful mind who has contributed a lot to econometrics and statistics. Another great way to support the project is by sharing it and :star: it!

A 2024 snapshot of this project is also published on the Universidad Rey Juan Carlos Institutional Repository: https://hdl.handle.net/10115/44997
