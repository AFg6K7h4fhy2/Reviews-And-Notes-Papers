# A Machine Learning-Aided Global Diagnostic And Comparative Tool To Assess Effect Of Quarantine Control In COVID-19 Spread

Proposed questions:

* How might we think about this in relation to: (a) parameteric characterization of unknown functional forms (e.g. "let quarantine strength be a sigmoid") and (b) more traditional "non-parametric" approaches?
* How can we (quantitatively, qualitatively) assess the value-added or not of a neural network approach relative to those other approaches?

From MathQR:

__Parametric Statistics__: The branch of statistics dealing with inference about parameters of a population on the basis of observations and measurements taken from a sample.

__Non-Parametric Methods__: Methods of inference that make no assumptions about the underlying population distribution. Non-parametric tests are often concerned with hypotheses about the median of a population and use the ranks of the observations.


## Summary

From the in-brief section of the paper:

::: {.bquote}
There is an urgent need to quantify the role played by quarantine policies implemented in various regions globally to curtail the spread of COVID-19. A model lying at the intersection of machine learning and epidemiology is shown to be powerful in diagnosing the quarantine policy evolution, which mimics well the real-time, on-ground situation seen in that region. The model, applied to 70 countries globally, is hosted publicly, making it a robust, useful tool in the fight against COVID-19.
:::

From the bigger picture section of the paper:

::: {.bquote}
As we enter the fifth month in the fight against COVID-19, it is evident that the government response to the COVID-19 pandemic has been spatially and temporally diverse. As such, the role played by the varying quarantine measures in different countries in shaping the infection growth curve is still not clear. To address this need, we have developed a novel model which lies at the intersection of the fields of epidemiology and machine learning and allows us to analyze and compare the role of quarantine control policies globally, across the continents of Europe, North America, South America and Asia (results hosted at
<https://covid19ml.org/>). Such a robust, publicly available tool can be of significant value for studies looking at the correlation between the quarantine strength evolution in a particular region with a wide range of metrics spanning from mortality rate to socio-economic landscape impact of COVID-19 in that region
:::

From the summary section of the paper:

::: {.bquote}
We have developed a globally applicable diagnostic COVID-19 model by augmenting the classical SIR epidemiological model with a neural network module. Our model does not rely upon previous epidemics like SARS/MERS and all parameters are optimized via machine learning algorithms used on publicly available COVID-19 data. The model decomposes the contributions to the infection time series to analyze and compare the role of quarantine control policies used in highly affected regions of Europe, North America, South America, and Asia in controlling the spread of the virus. For all continents considered, our results show a generally strong correlation between strengthening of the quarantine controls as learnt by the model and actions taken by the regions’ respective governments. In addition, we have hosted our quarantine diagnosis results for the top 70 affected countries worldwide, on a public platform.
:::

## Notes

* Updated confirmed global cases from 12,552,765 as of 12 July 2020?
* Why no quarantine in Sweden?
* "_The disparity of the countries' responses is compounded by commensurate disparity in their effectiveness in controlling the severity of infectious spread_"
* Recall Law Of Mass Action: "_the rate of change of compartment population at the next time step is proportional to the compartment population at the current time step._"
* Recall identifiability—uniquely determining parameters from data—in context of opting for more compartments over fewer.
* Recall independent estimation: _...using parameters based on previous knowledge of [phenomenon] and not derived independently from the [phenomenon] data or parameters_
* Model pitfall: _These models cannot capture the large-scale effects of more granular interactions, such as the population’s response to social distancing and quarantine policies._ How much information is needed here to result in a more granular approach being taken?
* Interesting note about NNs: "_Unbounded activation functions, in particular, such as the rectified linear unit (ReLU) has been known to be effective in approximating nonlinear functions with a finite set of parameters._"
* On deviation from compartmental model assumptions: "_An important assumption of the SIR models is homogeneous mixing among the sub-populations. Therefore, this model cannot account for social distancing or social network effects. In addition, the model assumes uniform susceptibility and disease progress for every individual; and that no spreading occurs through animals or other non-human means. Alternatively, the SIR model may be interpreted as quantifying the statistical expectations on the respective mean populations, while deviations from the model's assumptions contribute to statistical fluctuations around the mean_"
* $Q(t)$ is the time varying quarantine strength term, $T(t)$ is the quarantined population, $\delta$ is the recovery rate for the quarantined population
* COVID spread parameter, $C_p(t) = \frac{\beta}{\gamma + \delta + Q(t)}$. Note: ${C_p} > 1$ rapid disease spread, ${C_p} < 1$ disease under control.
* Quarantine efficiency: $Q_{\text{eff}} = Q(30) - Q(1)$ once the 500th infected case is detected. Why this?
* The model itself (54 tunable parameters):

* Q(t) include S, I, R, W but t

it's an "autonomous" system in ODE lingo



* Don't have reentering isolation, go out of quarantine to R not I.

<!-- Colleague 2's points

* Remove S, quarantine. Remove I, isolation. But in this case they remove I, but call it quarantine. They are actually modelling isolation, not quarantine.
* C(t) not really a time varying reproduction number. Non-specific effect reducing period of infectious people actually infecting people. So, $delta$ shouldn't be defined?
* Mixes up incidence and prevalence.
* Recursive NN, memory output, use recurrent NN; looks like Euler method with time set of time 1;

Colleague 1's points:

_so the idea of a "non-parameteric" way of "learning" functional responses from data is very appealing a priori_
We have some functional form. How quickly we are pulling people out of I. Initially we do not know much about testing. Finding infectious people before they infected people. Parameter = decide shape of curve and fit it. Or can decide to get data points and learn functional form with more flexible methods. Like putting a prior on Q(t) that is pretty vague across a bunch of different functional forms.

"to know where you're going, you just need to know where you (currently) are, not when you are "

mathematical epi. theoretical population biology dynamical systems world, autonomous v. non-autonomous

how to evaluate this + how to determine it is better.

Colleague 3's points:

* has seen post-processing layer
* regularizing mechanistic component.

NN(t) v. NN(S(t), I(t), R(t))
construct non-autonomous

What is being capture by NN(W, U)

General Dynamic Systems


NN v. Gaussian Process culture
	really the same world under certain limits
	non-parametric land practicality argument
		conceptual beauty not cared about
	natural uncertainty, none, predictive uncertainty, yes
	point estimate with this v. full bayesian inference
	George says one can use bootstrapping...

So much of life is working in the cave.
Not having knowledge.
Reading is so important.
It reveals far more than most can ever imagine.

Hyperprior on your weights.
Then use full Bayes.

Time aware but leave one out
Bayesian window shifts

Time structure problem, quite tricky: time aware cross validation


Setting up GitHub action for pre-commit autoupdate
branch before merge

How to think about blending ML and

Any do we evaluate whether we are blending them well?

Tension on within model and postprocessing  -->
