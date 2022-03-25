**Explanatory Variable**
Also known as the `independent` or `predictor variable`, it explains variations in the response variable; in an experimental study, it is manipulated by the researcher

**Response Variable**
Also known as the `dependent` or `outcome variable`, its value is predicted or its variation is explained by the explanatory variable; in an experimental study, this is the outcome that is measured following manipulation of the explanatory variable

![Responce and Explanatory variable](https://images.deepai.org/django-summernote/2019-06-18/fe2a668a-625f-431f-9472-e177d594ba2c.png)

**Example 1**

A team of veterinarians wants to compare the effectiveness of two fertility treatments for pandas in captivity. The two treatments are in-vitro fertilization and male fertility medications. This experiment has one explanatory variable: type of fertility treatment. The response variable is a measure of fertility rate.

`Factor variables` are categorical variables that can be either numeric or string variables. There are a number of advantages to converting categorical variables to factor variables.

## Model Selection

It is a process of selecting a model from a set of candidate models.

It can either be implicit or explicit in the following ways:
1.Hypothesis tests require selecting between a null hypothesis and alternative hypothesis model.
2.An auto-regressive model requires selecting the order p.
3.Selecting specific predictors.

A good model selection technique will balance `goodness of fit or simplicity`

Akaike Information Criterion(AIC) is a metric that is used to compare the fit of different regression models

**How do I interpret negative AIC values?**

> The lower the value for AIC, the better the fit of the model. The absolute value of the AIC value is not important. It can be positive or negative.

$$AIC = 2K - 2\,ln(L)$$

where:

- _K_: The number of model parameters.The default value of K is 2, so the model with just one prefictor will have value a K value of 2+1 = 3
- _$ln(K)$_: The log-likelihood of the model.

# References

[Understanding negative AIC values](https://www.statology.org/negative-aic/)
