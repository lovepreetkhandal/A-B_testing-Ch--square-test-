# A-B_testing-Ch--square-test

## Applying Chi-Square Test For Independence


### State Hypotheses & Acceptance Criteria For Test
The very first thing we need to do in any form of Hypothesis Test is state our Null Hypothesis, our Alternate Hypothesis, and the Acceptance criteria.

In the code above we code these in explcitly & clearly so we can utilise them later to explain the results. We specify the common Acceptance Criteria value of 0.05.

Calculate Observed Frequencies & Expected Frequencies
As mentioned in the section above, in a Chi-Square Test For Independence, the observed frequencies are the true values that we’ve seen, in other words, the actual rates per group in the data itself. The expected frequencies are what we would expect to see based on all of the data combined.

In the Code:

Summarises our dataset to a 2x2 matrix for signup_flag by mailer_type
Based on this, calculates the:
Chi-Square Statistic
p-value
Degrees of Freedom
Expected Values
Prints out the Chi-Square Statistic & p-value from the test
Calculates the Critical Value based upon our Acceptance Criteria & the Degrees Of Freedom
Prints out the Critical Value

Based upon our observed values, we can give this all some context with the sign-up rate of each group. We get:

Mailer 1 (Low Cost): 32.8% signup rate
Mailer 2 (High Cost): 37.8% signup rate
From this, we can see that the higher cost mailer does lead to a higher signup rate. The results from our Chi-Square Test will provide us more information about how confident we can be that this difference is robust, or if it might have occured by chance.

We have a Chi-Square Statistic of 1.94 and a p-value of 0.16. The critical value for our specified Acceptance Criteria of 0.05 is 3.84

Note When applying the Chi-Square Test above, we use the parameter correction = False which means we are applying what is known as the Yate’s Correction which is applied when your Degrees of Freedom is equal to one. This correction helps to prevent overestimation of statistical signficance in this case.

### Analysing The Results
At this point we have everything we need to understand the results of our Chi-Square test - and just from the results above we can see that, since our resulting p-value of 0.16 is greater than our Acceptance Criteria of 0.05 then we will retain the Null Hypothesis and conclude that there is no significant difference between the signup rates of Mailer 1 and Mailer 2.
