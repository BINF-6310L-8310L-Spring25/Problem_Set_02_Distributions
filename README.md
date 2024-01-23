# Problem_set_3

# Purpose

The purpose of this lab is to give you an intuition for the various distributions we covered in class. 

Since you will be asked to include figures you will see **true/false** questions in the canvas quiz. This will allow me to grade/comment on the individual questions. 

# Uniform distribution

Create a datatset drawn from a uniform distribution with 10,000 samples taken between the values of 4 and 6

## Question 1

Visualize that distribution with a histogram 



# Binomial Distribution 

If two mice who are carriers for albinism (but not albino themselves) mate, their offspring have a 1/4 probability of being albino. Based on this information conduct the following analyses

## Question 2

What is the probability that exactly 2 offspring in a litter of 10 are albino?

## Question 3

Plot the probability distribution function for albinism in a litter of 10 mice.

## Question 4

What is the probability that there are 8 or more albino mice in a litter of 10 mice?

## Question 5

What is the probability of at least 3 but no more than 5 albino mice in a litter of 10


# Multinomial Distribution 

Recall our Dihybrid cross in birds

<img src="https://user-images.githubusercontent.com/47755288/207365544-63e26fae-1325-4be0-9cfa-ee48048cc37a.png" width="300">

## Question 6

If the parental birds shown above have 20 offspring throughout their lifetime, what is the probability of getting equal numbers of Yellow/Normal, Yellow/Clear, White/Normal, and White/Clear offspring?

## Question 7

The White/Clear birds are the most valuable for your research. How many offspring should you plan for so that there is a >80% chance of having at least 8 White/Clear baby birds?


# Standard Normal Distribution

Recall our exploration of the Central Limit Theory. Imagine a school is trying to determine which classes are underperforming. 

To do this, they take the mean test scores from all student's standardized exams in the class. They show a normal distribution of mean scores and suggest that this indicates that differences in teacher performance are impacting student exams. At the school board meeting, there is a proposal to fire the teachers with the two lowest mean exam scores. 

You are worried that the test, and not the teachers, are at fault for some of the low scores. So, you do some reading on the standardized test given to students. You find this standardized test has an **error rate of 0.12**. Therefore, even if a student knows the answer, there is only an 88% chance they will correctly answer the question when they know the answer. The exam has 100 questions.

You want to know if low average classroom scores could be due to this error rate? So you assume every student knows the answer to the questions and the only reason students get the answer wrong is the random error rate on the exam. 

You set out to demonstrate this to the school board. 

## Question 8

You know that if the scores are based only on the random error, they should follow a binomial distribution. 

Take a sample of 31 student scores from the binomial distribution of a 100 question where the rate of success is random and 88%.  What is the mean score in that classroom?

## Question 9

There are 120 classes in the school district and they are all 31 students. Simulate 120 classrooms taking the exam and then plot the mean classroom score in a histogram. 

## Question 10

You note that this distribution looks like a normal distribution! From your sample of mean classroom scores across the district, calculate the mean and variance of the average classroom scores (from the 31 students.) 

## Question 11

Use the mean and variance of the mean classroom scores across the district to plot a normal distribution of scores under the assumption that all scores are due only to random error. 

## Question 12

Based on your model, you examine the two lowest scoring classrooms. Classroom A had a mean exam score of 87.5. Classroom B had a mean exam score of 80.4. Which classroom(s) could have obtained this mean score due simply to the error of the exam? 


# Chi-Squared Distribution

Using the Chi-Squared function in R report the following things

Chi-Squared Value at which 95% and 99% of values are below that value for

- 2 Degrees of Freedom
- 6 Degrees of Freedom
- 10 Degrees of Freedom


# T-Distribution

A teacher at a private school down the road heard about your work that showed that error alone could produce a normal distribution of average test scores. They decide to replicate your study. 

Their class sizes, however, are much smaller. There are 11 students in each class. There are also only 50 classes in the school. This means they need to use the T-Distribution instead of the Normal distribution to model their classroom mean scores. 

## Question 13

Plot the T-distribution for 50 classes (degrees of freedom) where the distribution is centered over the score 88. 

## Question 14

Based on your model, you examine the two lowest scoring classrooms in this school. Classroom A had a mean exam score of 87.5. Classroom B had a mean exam score of 80.4. Which classroom(s) could have obtained this mean score due simply to the error of the exam? 


# F-Distribution

As we have seen, the shape of the F-Distribution varies depending on which sample size is used in the numerator or denominator. You are conducting an analysis with sample sizes (12 and 31). You are trying to find the F-value at which 95% of values fall below this. 


# Question 15

Which degrees of freedom do you use in the numerator to ensure the test is the most conservative?




