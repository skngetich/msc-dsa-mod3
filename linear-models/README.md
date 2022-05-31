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

![Response and Explanatory
variable](https://images.deepai.org/django-summernote/2019-06-18/fe2a668a-625f-431f-9472-e177d594ba2c.png)

**Example 1**

A team of veterinarians wants to compare the effectiveness of two
fertility treatments for pandas in captivity. The two treatments are
in-vitro fertilization and male fertility medications. This experiment
has one explanatory variable: type of fertility treatment. The response
variable is a measure of fertility rate.

`Factor variables` are categorical variables that can be either numeric
or string variables. There are a number of advantages to converting
categorical variables to factor variables.

## Model Selection

It is a process of selecting a model from a set of candidate models.

It can either be implicit or explicit in the following ways:
1.Hypothesis tests require selecting between a null hypothesis and
alternative hypothesis model.  
2.An auto-regressive model requires selecting the order p.  
3.Selecting specific predictors.

A good model selection technique will balance
`goodness of fit or simplicity`

## Extensions of the linear models

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

### Interactions

Interaction help us to test for an influence between the response
variable as the relate to the common explanatory variable

-   `Main effect` = Coefficient for predictors used to main interaction
    terms
-   `Interaction effects` = coefficient for interaction terms
-   `State interaction` = polynomial interactions

#### Visualizing Interaction

-   *No interaction* - categories have the same slope
    coefficient(Parallel lines)
-   *Interaction -* categories do not have the same slope coefficient
    (non-parallel lines)

**NB:**

Given the regression formula
*C**a**l**o**r**i**e**s* = *β*<sub>0</sub> + *β*<sub>1</sub> × *C**a**r**b**s* + *β*<sub>2</sub> × *M**e**a**t* + *β*<sub>3</sub> × *C**a**r**b**s* \* *M**e**a**t*

where the p-value of Carbs is 0.0014, Meat is 0.7925 and the interaction
between Carbs and Meat is 0.00012.Meat cannot be removed since it is in
the significant interaction term.

**When to include interaction term**

1.  The interaction term should make sense conceptually.
2.  The interaction term should be statistically significant.

**(Step Function)\[<https://byjus.com/maths/step-function/>\]** also
called staircase function is defined as a piece wise function that has
only finite number of pieces

## Splines

linear regression imposes two key restrictions on the model.We assume
the relationship between the response and predictors is **Linear** and
**Additive**.

> an estimator *f̂*(*x*) is consistent if, as our sample size grows,
> *f̂*(*x*) converges to the true regression function
> *f*(*x*) = *E*(*Y*\|*X*=*x*)

> A **cubic spline** with knots as *x*-values is a continuous piecewise
> cubic polynomial with continuous derivates and continuous second
> derivatives as each knot

for **polynomial regression** we use **degree** while in **cubic
spline** we choose the **knots**

place more knots where *f* appears to be changing rapidly and place
fewer knots where *f* appears tobe slowly varying.

Splines are a nice way of modelling smoooth regression functions To
increase the flexibility of a spine , we increase the number of knots
Natural cubic splines allow us retain the model of complexity of a cubic
spline while adding two extra interior knots at the cost of restricting
our model to be linear outside the range of the observed data.

Smoothing splines enable us to avoid the problem of knot selection
altogether and instead specify a single patameter: the desired effective
degrees of freedom for fit.
