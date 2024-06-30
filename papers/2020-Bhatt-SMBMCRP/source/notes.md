
<!--
Define terms.
Quotes.
Questions you have.
Comments you have.
Research ideas / questions.
Examining sources.




Abstract,Conclusion
Claims
Terms
Red-Teaming AMAP
  Assuming All Claims Are Wrong
  What would it look like if This Other Thing?
  How does this matter more broadly?
Quotes
Resources Relevant

Comments To The Authors
Extensions Of The Equations
Future Work Potential
Readability

Possible Posts To Write From This
  Last Recorded:
-->


# Abstract & Conclusion

Claim, in one sentence:

>

The abstract:

> We propose a general Bayesian approach to modeling epidemics such as COVID-19. The approach grew out of speciﬁc analyses conducted during the pandemic, in particular an analysis concerning the effects of non-pharmaceutical interventions (NPIs) in reducing COVID-19 transmission in 11 European countries. The model parameterizes the time varying reproduction number Rt through a regression framework in which covariates can e.g. be governmental interventions or changes in mobility patterns. This allows a joint ﬁt across regions and partial pooling to share strength. This innovation was critical to our timely estimates of the impact of lockdown and other NPIs in the European epidemics, whose validity was borne out by the subsequent course of the epidemic. Our framework provides a fully generative model for latent infections and observations deriving from them, including deaths, cases, hospitalizations, ICU admissions and seroprevalence surveys. One issue surrounding our model’s use during the COVID-19 pandemic is the confounded nature of NPIs and mobility. We use our framework to explore this issue. We have open sourced an R package epidemia implementing our approach in Stan. Versions of the model are used by New York State, Tennessee and Scotland to estimate
the current situation and make policy decisions.

The conclusion:

> This article has discussed a class of statistical models for epidemics such as Covid-19 which are able to capture key epidemiological mechanisms. The model has appeared in various forms for speciﬁc analyses during the Covid-19 crisis and, at the time of writing, continues to be used to inform public policy. By presenting it in a general form and discussing key modelling difﬁculties we hope to stimulate discussion around it. One key difﬁculty within the framework is dealing with confounded variables, particularly those used to explain changes in transmission during the early stages of an epidemic. The analyses in Section 8 make a ﬁrst step in dealing with these, and support the central ﬁnding of Flaxman et al. (2020b): that lockdown and other NPIs together served to control the ﬁrst wave of the epidemic in 11 European countries.
>
> A number of model enhancements have not been discussed here. These include explicitly accounting for importations, and allowing for uncertainty in the generation and infection to observation distributions. The model can be ﬁt using Stan (Stan Development Team, 2018), but the adaptive Hamiltonian Monte Carlo used often has difﬁculty converging when latent infections are modeled directly, or when multiple regions are jointly modeled. We conjecture that convergence may be improved by carefully choosing initial parameters for the sampler. Future research could explore whether alternative samplers can be developed to ﬁt these models more pragmatically.

## Notes

* Why read this paper? Good introduction to people who are new(ish) to Renewal Modelling.


## What To Record?

* Every term you do not know or that you cannot define.
* Why does this paper matter?
* What lessons can be learned from this paper?
* Color code and label equations to make them real


## Test Questions

## Appendix

### Citations

```
@article{bhatt2023semi,
  title={Semi-mechanistic Bayesian modelling of COVID-19 with renewal processes},
  author={Bhatt, Samir and Ferguson, Neil and Flaxman, Seth and Gandy, Axel and Mishra, Swapnil and Scott, James A},
  journal={Journal of the Royal Statistical Society Series A: Statistics in Society},
  volume={186},
  number={4},
  pages={601--615},
  year={2023},
  publisher={Oxford University Press US}
}
```
