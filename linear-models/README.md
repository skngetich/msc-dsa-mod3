<<<<<<< HEAD
Linear models Notes
================

**Explanatory Variable**  
Also known as the `independent` or `predictor variable`, it explains
variations in the response variable; in an experimental study, it is
manipulated by the researcher

**Response Variable**  
Also known as the `dependent` or `outcome variable`, its value is
predicted or its variation is explained by the explanatory variable; in
an experimental study, this is the outcome that is measured following
manipulation of the explanatory variable
=======
**Explanatory Variable**
Also known as the `independent` or `predictor variable`, it explains variations in the response variable; in an experimental study, it is manipulated by the researcher

**Response Variable**
Also known as the `dependent` or `outcome variable`, its value is predicted or its variation is explained by the explanatory variable; in an experimental study, this is the outcome that is measured following manipulation of the explanatory variable
>>>>>>> 80e1715bb989e47d5df360d93d97110b6f06100f

![Response and Explanatory
variable](https://images.deepai.org/django-summernote/2019-06-18/fe2a668a-625f-431f-9472-e177d594ba2c.png)

**Example 1**

<<<<<<< HEAD
A team of veterinarians wants to compare the effectiveness of two
fertility treatments for pandas in captivity. The two treatments are
in-vitro fertilization and male fertility medications. This experiment
has one explanatory variable: type of fertility treatment. The response
variable is a measure of fertility rate.

`Factor variables` are categorical variables that can be either numeric
or string variables. There are a number of advantages to converting
categorical variables to factor variables.

=======
A team of veterinarians wants to compare the effectiveness of two fertility treatments for pandas in captivity. The two treatments are in-vitro fertilization and male fertility medications. This experiment has one explanatory variable: type of fertility treatment. The response variable is a measure of fertility rate.

`Factor variables` are categorical variables that can be either numeric or string variables. There are a number of advantages to converting categorical variables to factor variables.

>>>>>>> 80e1715bb989e47d5df360d93d97110b6f06100f
## Model Selection

It is a process of selecting a model from a set of candidate models.

It can either be implicit or explicit in the following ways:
<<<<<<< HEAD
1.Hypothesis tests require selecting between a null hypothesis and
alternative hypothesis model.  
2.An auto-regressive model requires selecting the order p.  
3.Selecting specific predictors.

A good model selection technique will balance
`goodness of fit or simplicity`

## Extentions of the lineat models

Linear model have highly restrictive assumptions:

-   There is a linear and additive relationship between the response and
    the predictor.  
-   additive assumptions means that the effect of changes in a predictor
    *X*<sub>*j*</sub> on the response *Y* is independent of the values
    of the other predictors.

### Removing the additive assumption

Consider
*Y* = *β*<sub>0</sub> + *β*<sub>1</sub>*X*<sub>1</sub> + *β*<sub>2</sub>*X*<sub>2</sub> + *ϵ*

The model can be extended by adding `an interaction term` which is
constructed by computing the pr product of *X*<sub>1</sub> and
*X*<sub>2</sub>. This result in the model
*Y* = *β*<sub>0</sub> + *β*<sub>1</sub>*X*<sub>1</sub> + *β*<sub>2</sub>*X*<sub>2</sub> + *ϵ*
=======
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


#Pricipal Componentn Analysis  
Dimension-reduction tool that can be use to reduce  a large set of variables to a small set that still contains most of the information in the large set.

PCA is for interpretation and visualization in fewer dimensional space.

PCA is one of the techniques used for dimension reductions.

![PCA](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.javatpoint.com%2Fdimensionality-reduction-technique&psig=AOvVaw3Q3RwcqodbUwqbJ-n9AjhG&ust=1648308068199000&source=images&cd=vfe&ved=0CAsQjRxqFwoTCKDa0qvI4fYCFQAAAAAdAAAAABAJ)



# References

[Understanding negative AIC values](https://www.statology.org/negative-aic/)
>>>>>>> 80e1715bb989e47d5df360d93d97110b6f06100f
