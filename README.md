# Resources on Causal Inference
"Correlation is not Causation." But when is association causation? How do we deal with observational data when the randomization of treatment is not possible? These questions have motivated me to spend this summer diving deep into the causal inference literature. Here are some of the resources that I found useful (and my reviews) if you are interested in this topic.
## Books
1. [Causal Inference for The Brave and True](https://matheusfacure.github.io/python-causality-handbook/landing-page.html) - Matheus Facure
2. [Causal Inference in Python](https://www.oreilly.com/library/view/causal-inference-in/9781098140243/) - Matheus Facure
3. [Causal Inference The MixTape](https://mixtape.scunning.com/) - Scott Cunningham
4. [The Book of Why](http://repo.darmajaya.ac.id/5342/1/The%20book%20of%20why_%20the%20new%20science%20of%20cause%20and%20effect%20%28%20PDFDrive%20%29.pdf) - Dana Mackenzie and Judea Pearl
5. [Causality: Models, Reasoning and Inference](https://bayes.cs.ucla.edu/BOOK-2K/neuberg-review.pdf) - Judea Pearl

   Not an easy text to read because it is very theoretical and the language is not very beginner-friendly. But it is a great start to learning about the graphical representation of causal relationships. Some important concepts you'll learn are closing back-door paths, minimally sufficient adjustment sets, and Bayesian networks.
7. [The Effect: An Introduction to Research Design and Causality](https://theeffectbook.net/) - Nick Huntington-Klein

   A very comprehensive and light-hearted text on causal inference. I see it as a guidebook on the topic whenever I want to refresh my memory on certain concepts.
## Research Papers
1. [Understanding Propensity Score Analyses
](https://www.redjournal.org/article/S0360-3016(20)30888-9/fulltext#%20) - Lalani, Nafisha, et al.

It was a little confusing for me when I first learned about propensity scores, especially when looking at the graphical model. As I have mentioned, there will be many adjustment sets that you can condition on to block the backdoor paths and you can choose either one of them. The propensity score is the probability of receiving the treatment. Therefore, we only include covariates that we suspect might affect the receiving of treatment in the propensity score model. For example, even though by looking at the adjustment set, variable A should be controlled for to block the backdoor path, we need to question ourselves to see if variable A also affects the probability of receiving the treatment for all the units. 

2. [Variable selection for propensity score modes](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1513192/) - Brookhart, M. Alan, et al.
## Python Libraries
1. [CausalInference](https://pypi.org/project/CausalInference/)
2. [causallib](https://pypi.org/project/causallib/)
3. [DoWhy](https://www.pywhy.org/dowhy/v0.11.1/)
4. [CausalML](https://causalml.readthedocs.io/en/latest/about.html)
