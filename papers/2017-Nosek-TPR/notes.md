# The Preregistration Revolution

<!--
Define terms.
Quotes.
Questions you have.
Comments you have.
Research ideas / questions.
Examining sources.

For this [essay], I read the following with notes, read the following,
skimmed the following.
(N, R, S)
For these references, I find the abstract this % adequate:
~100%, 90%, ..., 10%, 5%. (log scale based on number of inadequacies)
How much a single inadequacies compromise their contribution or results.
Inadequacies include wrong measurements or definitions.
-->



__Questions And Note On The Topic Of Pre-Registration And On This Paper Proposed By My Team Lead__

* How true is the statement: "_Forecasting is the strongest form of preregistration._"
* How should we think about the value of preregistration and or the forecasting problem in non-NHST (null-hypothesis significance testing) contexts?

Regarding this paper:

> This paper focuses on NHST [null hypothesis significance testing] because of its pervasive use (e.g., refs. 28 and 29). The opportunities and challenges discussed are somewhat different with other statistical approaches, such as Bayesian methods. However, no statistical method on its own avoids researcher opportunity for flexibility in analytical decisions, such as exclusion criteria or the creation of variables (30).

## Abstract & Conclusion

Claim, in one sentence:

>  Widespread adoption of preregistration will increase distinctiveness between hypothesis generation and hypothesis testing and will improve the credibility of research findings.

The abstract:

> Progress in science relies in part on generating hypotheses with existing observations and testing hypotheses with new observations.This distinction between postdiction and prediction is appreciated conceptually but is not respected in practice. Mistaking generation of postdictions with testing of predictions reduces the credibility of research findings. However, ordinary biases in human reasoning,such as hindsight bias, make it hard to avoid this mistake. An effective solution is to define the research questions and analysis plan before observing the research outcomes—a process called preregistration. Preregistration distinguishes analyses and outcomes that result from predictions from those that result from postdictions. A variety of practical strategies are available to make the best possible use of preregistration in circumstances that fall short of the ideal application, such as when the data are preexisting. Services are now available for preregistration across all disciplines, facilitating a rapid increase in the practice. Widespread adoption of preregistration will increase distinctiveness between hypothesis generation and hypothesis testing and will improve the credibility of research findings.

The conclusion:

> Sometimes researchers use existing observations of nature to generate ideas about how the world works. This is called post-diction. Other times, researchers have an idea about how the world works and make new observations to test whether that idea is a reasonable explanation. This is called prediction. To make confident inferences, it is important to know which is which.Preregistration solves this challenge by requiring researchers to state how they will analyze the data before they observe it,allowing them to confront a prediction with the possibility of being wrong. Preregistration improves the interpretability and credibility of research findings.

## Glossary

__Prediction__

__Postdiction__

__Hypothesis-Testing__: ...testing those [previously generated (off of existing data)] hypotheses by obtaining new observations [pp. 2600]

__Hypothesis-Generation__: ... generating hypotheses based on existing observation... [pp. 2600]

__Post Hoc Theorizing__:

__Science__

__Hypothesis__

__Null Hypothesis__: In NHST, one usually compares a null hypothesis of no relationship among the variables and an alternate hypothesis in which the variables are related. Data are then observed that lead to rejection or not of the null hypothesis. Rejection of the null hypothesis at $P < 0.05$ is a claim about the likelihood that data as extreme or more extreme than the observed data would have occurred if the null hypothesis were true. [pp. 2601]

__Significance Testing__

__Cognitive Bias__

__Hindsight Bias__:

__Preregristration__: ...committing to analytic steps without advance knowledge of the research outcomes. [...] With preregistration, prediction is achieved because selection of tests is not influenced by the observed data, and all conducted tests are knowable. [pp. 2601]

## Notes

### [pp. 2600]

* "_This distinction between postdiction and prediction is appreciated conceptually but is not respected in practice."_: Why? There are many different scenarios for experimentation, each with their own difficulties, I have trouble understanding why more scientists have been unable to rigorously comparmentalize their topics of study. A language of experimental setup (perhaps something like a collection of flowcharts) seems possible for the natural sciences and could aid with proper experimental design and procedure.
  * See two sentence down: "_An effective solution is to define the research questions and analysis plan before observing the research outcomes—a process called preregistration._"
* Here is a really nice description of the scientific workflow: "_Progress in science is marked by reducing uncertainty about nature. Scientists generate models that may explain prior observations and predict future observations. Those models are approximations and simplifications of reality. Models are iteratively improved and replaced by reducing the amount of prediction error. As prediction error decreases, certainty about what will occur in the future increases._"
* George Box’s aphorism: "_All models are wrong but some are useful_"
* Continuing on the production of science and distinctions in modes of research: "_Scientists improve models by generating hypotheses based on existing observations and testing those hypotheses by obtaining new observations. These distinct modes of research are discussed by philosophers and methodologists as hypothesis-generating versus hypothesis-testing, the context of discovery versus the context of justification, data-independent versus data-contingent analysis, and exploratory versus confirmatory research_"
* What is a postdiction? Briefly, generating hypothesis based on existing data or observations. These hypotheses are directly at questions like "why does thing have its properties?".
* What is a prediction? Briefly, the testing of hypothesis via the collection of new observation about what might occur, answering questions akin to "what properties will this thing have?".
* Why is testing predictions important? _Testing predictions assesses the uncertainty of scientific models by observing how well the predictions account for new data._
* Why is not distinguishing postdictions from predictions harmful?: "_Presenting postdictions as predictions can increase the attractiveness and publishability of findings by falsely reducing uncertainty. Ultimately, this decreases reproducibility_"
  * [TODO, Example] An example that: A meteorologist wants to understand cloud formation. The meteorologist has a model of cloud formation, using data from region A, but wants to now study region A. Given the meteorologist's initial, unvalidated understanding of region B, they hypothesize that their model describes cloud formation with approximately the same accuracy as in region A. This hypothesis is their postdiction.
  * How is failing to distinguish between postdictions and predictions a failure of reasoning?: "_It is an example of circular reasoning—generating a hypothesis based on observing data, and then evaluating the validity of the hypothesis based on the same data_"
* What is hindsight bias?: "_With hindsight bias, the observer uses the data to generate an explanation, a postdiction, and simultaneously perceives that they would have anticipated that explanation in advance, a prediction._"

### [pp. 2601]

* Very nice section on human bias, the effects of incentives in academia and science, and more: "_The values of impartiality and objectivity are pervasive (16), particularly for scientists, but human reasoning is not reliably impartial or objective (17, 18). Scientists are motivated to advance knowledge; scientists are also motivated to obtain job security, awards, publications, and grants. In the present research culture, these rewards are more likely to be secured by obtaining certain kinds of research outcomes over others. Novel results are rewarded more than redundant or incremental additions to existing knowledge. Positive results––finding a relationship between variables or an effect of treatments on outcomes––are rewarded more than negative results––failing to find a relation-ship or effect; clean results that provide a strong narrative are rewarded more than outcomes that show uncertainty or exceptions to the favored narrative (9, 19–21). Novel, positive, clean results are better results both for reward and for launching science into new domains of inquiry. However, achieving novel,positive, clean results is a rare event. Progress in research is halting, messy, and uncertain. The incentives for such results combined with their infrequency create a potential conflict of interest for the researcher. If certain kinds of results are more rewarded than others, then researchers are motivated to obtain results that are more likely to be rewarded regardless of the accuracy of those results._"
* On the abundance of different statistical tests and what this means for diagnosticity: "_The diagnosticity of a P value is partly contingent on knowing how many tests were performed (27)_." and "_If there were only one inference test to perform and only one way to conduct that test, then the P value is diagnostic about its intended likelihood. It is not hyperbole to say that this almost never occurs._"
* How does one correct for the number of tests that were actually conducted?
  * [TODO, Example]
* Here is a nice analogy on selecting different statistical tests based on observing different data: "_Gelman and Loken (37) refer to the problem as the garden of forking paths. There are a vast number of choices for analyzing data that could be made. If those choices are made during analysis, observing the data may make selecting some paths more likely and others less likely. By the end, it may be impossible to estimate the paths that could have been selected if the data had looked different or if analytic decisions were influenced by hindsight, confirmation,and outcome biases. This leaves the observed P values with unknown diagnosticity, rendering them uninterpretable. In other words, NHST cannot be used with confidence for postdiction_"
* On how researchers' degree of freedoms generates less accurate results, on average: _"Moreover, researchers have substantial degrees of freedom to conduct many different tests, and selection of those that yield positive results over those that yield negative results will increase the likelihood of attractive results at the expense of accuracy (30, 41, 42)._"
* What is preregistration? "_...committing to analytic steps without advance knowledge of the research outcomes. [...] With preregistration, prediction is achieved because selection of tests is not influenced by the observed data, and all conducted tests are knowable._"

### [pp. 2602]

* My expectation is that despite, preregistration, those less committed to the process will still attempt, mostly not out of malice but out of convenience, to avoid the checks in place with preregistration, especially when it comes to forgetting the original purpose of the study should more novel-ish findings present themselves.
* What is the ideal preregistration scenario?: "_A scientist makes observations in the world and generates a research question or hypothesis from those observations. A study design and analysis plan are created to evaluate that question. Then data are collected according to the design and analyzed according to the analysis plan. This confronts the hypothesis by testing whether it predicts the outcomes of the experiment. Following that, the researcher might explore the data for potential discoveries that generate hypotheses or potential explanations after the fact. The most interesting postdictions are then converted into predictions for designing the next study and the cycle repeats. In this idealized model, preregistration adds very little burden––the researcher just posts the study design and analysis plan to an independent registry before observing the data and then reports the outcomes of the analysis according to that plan._"
* How can discovery of assumption violations during analysis be addressed: define stages of preregistration, blind the dataset, preregister a decision tree, or define standard operating procedures (SOPs).



### Final Thoughts

In general, this paper describes, in very clear terms, the scientific method, and as such, stands as a concise but potent reference for those who are unfamiliar with what science actually consists of.

Stopped notes after: Preregistration Distinguishes Prediction and Postdiction

## Appendix

### Citation

```
@article{nosek2018preregistration,
  title={The preregistration revolution},
  author={Nosek, Brian A and Ebersole, Charles R and DeHaven, Alexander C and Mellor, David T},
  journal={Proceedings of the National Academy of Sciences},
  volume={115},
  number={11},
  pages={2600--2606},
  year={2018},
  publisher={National Acad Sciences}
}
```

### Comprehension Test & Questions

1. Define prediction.
2. Define postdiction.
3. Define hindsight bias.
4. What are examples of scientists' impartiality?
5. What sorts of scientific results are incentivized, generally speaking?
6. What is NHST designed for?
7. Create an example of a misused
8. What are some failures of preregistration?
9. What are some benefits of preregistration?
10. Why will "inferences from preregistered analyses be more reproducible than NHST analyses that were not preregistered"?: "because the relation between the analysis choices and findings cannot be influenced by motivation, memory, or reasoning biases."
11. What are some challenges with preregistration?


# Modest Pre-Registration

## Summary

https://statmodeling.stat.columbia.edu/2023/12/04/modest-preregistration/


## Notes


# Exploring Pre-Registration For Predictive Modeling

## Summary

https://statmodeling.stat.columbia.edu/2023/12/06/exploring-preregistration-for-predictive-modeling/


## Notes


# Of Course Its Preregistered. Just Give Me A Sec

## Summary

https://statmodeling.stat.columbia.edu/2023/11/21/of-course-its-preregistered-just-give-me-a-sec/
## Notes
