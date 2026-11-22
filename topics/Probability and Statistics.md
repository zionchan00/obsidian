Modelling Mindset - goes over diff school of probability/stats and when to use which
The Book of Why: The New Science of Cause and Effect is very good intro
Introduction to SLR (lectures here https://www.r-bloggers.com/2014/09/in-depth-introduction-to-machine-learning-in-15-hours-of-expert-videos/, https://mcmasteru365.sharepoint.com/:w:/s/sci-course-outlines/EVigYZ1rvklEm6iuA0SkY2YBtXn_oXAFGJQnNmm9St-y_w?rtime=-dKPhP3s2kg course based on ISLR here), Applied Predictive Modelling After, ESLR, Computer Age Statistical Inference: Algorithms, Evidence, and Data Science (goes over application across all schools and is historical too)
https://math.mit.edu/academics/undergrad/major/course18/applied.html MIT math curriculum
- Probability curriculum
	- [[ Introduction to Probability]] - hwang. https://projects.iq.harvard.edu/stat110/home 
	- Probabiility, Random Varaibles and Stochastic Porcesses - taleb says this is the best intro to probabiltiy for non-scientists
	- Bayesian
		- Probability Theory - the Logic of Science 
			- 1) Luce and Raiffa's _Games and Decisions_ (1989) introduces von Neumann and Morgenstern's axioms of objective utility theory and game theory; the book is geared towards serious social scientists.
			- 2) Savage's _The Foundations of Statistics_ (1954) is much harder than Luce and Raiffa, but it introduces an axiomatic system of subjective utility theory that complements objective utility theory well.
			- Fagin, Halpern, Moses and Vardi's _Reasoning About Knowledge_ (2004) contains a reasonable introduction to statistics via the Kolmogorov axiomatization. It is suitable for technically minded philosophy students who have no background in measure theory, set theory or analysis.
			- Modern statistics builds heavily on calculus. You may want to brush up - I really like Bressoud's _A Radical Approach to Real Analysis_ (2006). If you find yourself into the Kolmogorov axiomatization, you should also check out Bressoud's _A Radical Approach to Lebesgue Measure Theory_ (2008).
			- These books should give you some perspective on the different traditions in philosophy of statistics and rational decision theory. After this Jaynes should make a lot of sense - he belongs to the "subjective" camp that Savage pioneered. However, it is important to understand when studying philosophy of statistics that there are multiple camps and they have different perspectives.
		- Gelman's _Bayesian Data Analysis,_: guide to actual practice using R. It's a reference-book, nto a theory book
	- Frequentist
		- An Introduction to Probability Theory and Its Applications
	- 1000 exercises in probability
- Statistics curriculum
	- Statistical models: theory and practice. freedman, taleb recommendsan
- Causality curriculum
	- Judea Pearl's Causality
	- Causation, prediction, and search
https://www.foreignobjekt.com/post/anna-longo-probability-and-decision-theory
https://psyarxiv.com/39q8y/
Computer Age Statistical Inference: Algorithms, Evidence, and Data Science. goes through history of statistical methods
Modelling Extremaal Events - Taleb says this is the bible for thi stopic
probability theory -varadha. recommenddd by taleb for proofs of rpobability
- Frequentist vs Bayesian Debate
	- Recently was in the car with davidchen and talking about modelling cancer mutation through statistical inference.
	- What are probabilities? They're estimates of what the future will be. If we had a perfect understanding of how the future played out, we wouldn't need to think in probabilities - we could say with 100% certainty what would unfold. In this framing, referred to as the Bayesian framing as put forth by E.T Jaynes, probabilities are not inherent to the phenomena in question but to the mind that does the prediction. The opposing view is the inverse, the frequentist framing, which was what I learned in school.
	- A classic beginner probability problem is the biased coin, which over a very large number of flips, tends to land on one side more than the other. The fair coin in contrast should land near 50/50. What's the probability that the coin will land heads on the next flip?
	- The frequentist, who believes probability is inherent to the coin, would argue it can't be 0.5! After all, over a large enough number of flips, the coin is going to be either more or less likely to land heads over tails, not equal.
	- The Bayesian, who understands that probability is a function of understanding, would bet it's 0.5. We don't know which way the coin is biased, so the safe bet is to bet that it's 1.
	- It's true that the coin is more likely to land on one side than the other. But that statistical likelihood, a representation of 'indeterminacy', is the result of an actual deterministic process. If the hand that holds the coin holds it in such a way that they flip it onetime, does it
	- Is one of your two children a boy vs is your eldest child a boy. The first should yield an answer of 3/4 (boy/girl,girl/boy,boy/boy) and the second should yield an answer of 1/2. The first accounts for realities where the oldest or youngest is a boy. But the second only yields 1/2, and swithcing it to the chances that the youngest is a boy also only yields 1/2.  The difference is that the latter makes an assumption on the information available - we're given more information, so the nature of the bet changes.±
	- Let's say I have 4 cards and two are drawn at random
		- ace of hearts
			- ace of spades
			- two of hearts
			- two of spades
		- ace of spades
			- two of hearts
			- two of spades
			- ace of hearts
		- two of hearts
		- two of spades
	- One of them is an ace. What's the chance that another is also an ace?
		- ace of hearts <> two of hearts, ace of hearts <> two of spades, ace of hearts <> ace of spades
		- ace of spades <> two of spades, ace of spades <> two of hearts, and ace of spades <> ace of hearts cannot be a possibility because only ONE of them can be chosen first
		- 1/5
	- One of them is an ace of spades. Chances of holding an ace of hearts? In other words, chances that we hold two aces?
		- 1/3
		- 1/3*3/3
	- So there's an apparent contradiction between these two probabilities: 1/3 vs 1/5, when both seem to be asking nearly the same thing: what are the chances that we hold two aces?
	- Probabilities will change based on available information. When we don't know what ace the first card we have selected is as in the first probability, we have to factor in the possibility that the first of the two cards could be the other ace, unlocking a new tree of combinations. Why it seems to be contradictory because the first thing my mind did was think of the probability as reflective of the cards. Once I began thinking about it as a function of available information, it made sense!