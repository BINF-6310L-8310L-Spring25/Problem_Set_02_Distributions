# Problem_set_2

# Purpose

The purpose of this lab is to give you an intuition for the various distributions we covered in class. 

For reproducibility, please include the following command at the beginning of your code
```set.seed(123)```

Since you will be asked to include figures you will see **true/false** questions in the canvas quiz. This will allow me to grade/comment on the individual questions. 

&nbsp;

# Uniform distribution

Create a dataset drawn from a uniform distribution with 10,000 samples taken between the values of 4 and 6

### Question 1

Visualize that distribution with a histogram 

&nbsp;

# Binomial Distribution 

If two mice who are carriers for albinism (but not albino themselves) mate, their offspring have a 1/4 probability of being albino. Based on this information, conduct the following analyses

### Question 2

What is the probability that exactly 3 offspring in a litter of 10 are albino?

### Question 3

Plot the probability distribution function for albinism in a litter of 10 mice.

### Question 4

What is the probability that there are more than 7 albino mice in a litter of 10 mice?

### Question 5

What is the probability that there are 7 or more albino mice in a litter of 10 mice?
&nbsp;

# Multinomial Distribution 

Recall our Dihybrid cross in birds

<img src="https://user-images.githubusercontent.com/47755288/207365544-63e26fae-1325-4be0-9cfa-ee48048cc37a.png" width="300">

### Question 6

If the parental birds shown above have 20 offspring throughout their lifetime, what is the probability of getting equal numbers of Yellow/Normal, Yellow/Clear, White/Normal, and White/Clear offspring?

### Question 7

The White/Clear birds are the most valuable for your research. How many offspring should you plan for so that there is a >90% chance of having 8 or more (aka greater than 7) White/Clear baby birds?

&nbsp;

# Standard Normal Distribution

Recall our exploration of the Central Limit Theory. Imagine a school is trying to determine which classes are underperforming. 

To do this, they take the mean test scores from all student's standardized exams in the class. They show a normal distribution of mean scores and suggest that this indicates that differences in teacher performance are impacting student exams. At the school board meeting, there is a proposal to fire the teachers with the two lowest mean exam scores. 

You are worried that the test, and not the teachers, are at fault for some of the low scores. So, you do some reading on the standardized test given to students. You find this standardized test has an **error rate of 0.12**. Therefore, even if a student knows the answer, there is only an 88% chance they will correctly answer the question when they know the answer. The exam has 100 questions.

You want to know if low average classroom scores could be due to this error rate? So you assume every student knows the answer to the questions and the only reason students get the answer wrong is the random error rate on the exam. 

You set out to demonstrate this to the school board. 

### Question 8

You know that if the scores are based only on the random error, they should follow a binomial distribution. 

Take a sample of 31 student scores from the binomial distribution of a 100 question where the rate of success is random and 88%.  What is the mean score in that classroom?

### Question 9

There are 120 classes in the school district and they are all 31 students. Simulate 120 classrooms taking the exam and then plot the mean classroom score in a histogram. 

### Question 10

You note that this distribution looks like a normal distribution! From your sample of 120 mean classroom scores across the district, calculate the mean and standard deviation of the average classroom scores (from the 31 students.) 

### Question 11

Use the mean and standard deviation of the mean classroom scores across the district to plot a normal distribution of scores under the assumption that all scores are due only to random error. 

This would be your expected normal distribution for mean classroom scores if the individual grades are sampled from a random binomial distribution. 

### Question 12

The district wants to penalize teachers with an average classroom score of 87. What is the probability that a mean classroom score of 87 would be drawn from our normal distribution of mean (and binomially generated) test scores?

Would you recommend a mean classroom score of 87 as the starting score for penalizing teachers? 

&nbsp;

# Chi-Squared Distribution

Using the Chi-Squared function in R report the following things

### Question 13

Chi-Squared Value at which 95% of values are below this threshold for

- 2 Degrees of Freedom
- 6 Degrees of Freedom
- 10 Degrees of Freedom
- 100 Degrees of Freedom

&nbsp;

# T-Distribution

You are studying the effect of caffeine on sleep quality. You know that the mean hours of sleep for all adults is 7.2 hours. You sample 12 people who use caffeine after 3pm and find that their mean hours of sleep is 6 hours with a standard deviation of 1 hour. 

### Question 14

Based on the typical adult sleep schedule (7.2 hours), what is the probability that you would sample 12 individuals who have an average of 6 hours with a standard deviation of 1 hour?

### Question 15

You sample another 12 people who don't use caffeine after 3pm and find that their mean hours of sleep is 6.5 hours with a standard deviation of 1.5 hours. What is the probability you would sample this group from the typical adult population? 

&nbsp;

# F-Distribution

As we have seen, the shape of the F-Distribution varies depending on which sample size is used in the numerator or denominator, but what does this actually mean? 

You conducted two analyses (A and B)

Analysis A includes 100 samples and a variance of 20
Analysis B includes 15 samples and a variance of 40

### Question 16

You decide to put analysis B in the denominator. 
Calculate the F-value (proportion of the variances).
What is the probability that you would sample an F-value where the variance of A is less than 20? 

### Question 17

You decide to put analysis A in the denominator. 
Calculate the F-value (proportion of the variances).
What is the probability that you would sample an F-value where the variance of A is less than 20? 

