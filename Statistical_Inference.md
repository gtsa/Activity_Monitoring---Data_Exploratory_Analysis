## Probability
In this module we discuss probability, the foundation of statistical analysis. 
Probability assigns a number between 0 and 1 to events to give a sense of the "chance" of the event.
Probability has become our default model for apparently random phenomena. Our eventual goal is to use probability models,
our formal mechanism for connecting our data to a population. However, before we get to probability models,
we need to understand the basics of probability calculus. The next few lectures cover these basics.

## Conditional probability
Conditional probability is a very intuitive idea, "What is the probability given partial information about what has occurred?".
The probability of getting hit by lightning is small. However, it's much larger for people playing outside in open fields during a lightning storm!
In these lectures we go over the formal rules of conditional probability.

## Expected values
The empirical average is a very intuitive idea; it's the middle of our data in a sense. But, what is it estimating?
We can formally define the middle of a population distribution. This is the expected value.
Expected values are very useful for characterizing populations and usually represent the first thing that we're interested in estimating.

## Variability
An important characterization of a population is how spread out it is. One of the key measures of spread is variability.
We measure population variability with the sample variance, or more often we consider the square root of both, called the standard deviation.
The reason for taking the standard deviation is because that measure has the same units as the population.
So if our population is a length measurement in meters, the standard deviation is in meters (whereas the variance is in meters squared).

Variability has many important uses in statistics. First, the population variance is itself an intrinsically interesting quantity that we want to estimate.
Secondly, variability in our estimates is what makes them not imprecise. An important aspect of statistics is quantifying the variability in our estimates.

## Distributions
Some probability distributions are so important that we need to internalize their characteristics.
In these lectures we cover the most important probability distributions.

## Asymptotics
Asymptotics are an important topics in statistics. Asymptotics refers to the behavior of estimators as the sample size goes to infinity.
Our very notion of probability depends on the idea of asymptotics. For example, many people define probability as
the proportion of times an event would occur in infinite repetitions. That is, the probability of a head on a coin is 50%
because we believe that if we were to flip it infinitely many times, we would get exactly 50% heads.

We can use asymptotics to help is figure out things about distributions without knowing much about them to begin with. 
A profound idea along these lines is the Central Limit Theorem. It states that the distribution of averages is often normal,
even if the distribution that the data is being sampled from is very non-normal. This helps us create robust strategies
for creating statistical inferences when we're not willing to assume much about the generating mechanism of our data.

## Confidence intervals
When we estimate something using statistics, usually that estimate comes with uncertainty.
Take, for example, election polling. When we get a polled percentage of voters that favor a candidate,
we were only able to sample a small subset of voters. Therefore, our estimate has uncertainty associated with it.

Confidence intervals are a convenient way to communicate that uncertainty in estimates.

## Hypothesis testing
Deciding between two hypotheses is a core activity in scientific discovery. 
Statistical hypothesis testing is the formal inferential framework around choosing between hypotheses.

## P-values
P-values are a convenient way to communicate the results of a hypothesis test. When communicating a P-value,
the reader can perform the test at whatever Type I error rate that they would like.
Just compare the P-value to the desired Type I error rate and if the P-value is smaller, reject the null hypothesis.

Formally, the P-value is the probability of getting data as or more extreme than the observed data in favor of the alternative.
The probability calculation is done assuming that the null is true.
In other words if we get a very large T statistic the P-value answers the question
"How likely would it be to get a statistic this large or larger if the null was actually true?".
If the answer to that question is "very unlikely", in other words the P-value is very small,
then it sheds doubt on the null being true, since you actually observed a statistic that extreme.

## Power
We've talked about a Type I error, rejecting the null hypothesis when it's true.
We've structured our hypothesis test so that the probability of this happening is small.
The other kind of error we could make is to fail to reject when the alternative is true (Type II error).
Or we might think about the probability of rejecting the null when it is false. This is called Power = 1 - Type II error.
We don't have as much control over this probability, since we've spent all of our flexibility guaranteeing that the Type I error rate is small.

One avenue for the control of power is at the design phase. There, assuming our finances let us,
we can pick a large enough sample size so that we'd be likely to reject if the alternative is true.
Thus the most frequent use of power is to help us design studies.

## Resampling
Resampling based procedures are ways to perform population based statistical inferences, while living within our data.
Data Scientists tend to really like resampling based inferences, since they are very data centric procedures,
they scale well to large studies and they often make very few assumptions.
