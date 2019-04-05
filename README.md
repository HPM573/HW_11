# Homework Assignment 10

**Note**: Feel free to use any part of code from the 
[solution](https://github.com/HPM573/HW_4_Solution) to 
the [homework assignment 4](https://yale.instructure.com/courses/43583/assignments/92544).


**Overview**. For the Atrial fibrillation model you developed in 
[homework assignment 4](https://github.com/HPM573/HW_4_Solution), 
we want to investigate the performance of anticoagulation 
using cost-utility and cost-benefit methods.

**Problem 1: Modeling the effect of anticoagulation (Weight 1)**. 
Assume that the anticoagulation relative risk in reducing stroke incidence while in “Post-Stroke” is 0.65 and 
its relative risk in increasing mortality due to bleeding is 1.05. 
Calculate the transition probability matrix for this scenario where patients will 
receive anticoagulation while in state “Post-Stroke”. 
Make sure that the sum of probabilities in each row is 1.


**Problem 2: Discounted Cost and Utility (Weight 1)**. 
To measure the health impact of anticoagulation, 
we are assuming that the health utility of being in states 
“Well”, “Post-Stroke” and “Dead” are 1, 0.9, and 0, respectively. 
Let’s assume that experiencing a stroke reduces the patient’s utility to 0.2 for 1 week. 
Since in our model patients who had stroke moves to the state “Stroke” and 
stay there for 1 year (this is our model’s cycle length), 
we can approximate the patient’s utility while in state “Stroke” as: 

(utility during a week after stroke) × (proportion of cycle length in one week after stroke) + (utility of being in post-stroke) × (proportion of cycle length in post-stroke)
= 0.2 * 1/52 + 0.9 * 51/52 = 0.8865.

Use 0.8865 for the utility of being in “Stroke” when the cycle length 
is chosen to be 1 year. 
To calculate cost, we make the following assumptions: 
the cost incurred due to a stroke is $5,000, 
the annual cost of being in the post-stroke state is $200, and 
the annual cost of anticoagulation is $2000.
Use your simulation model to estimate the discounted total cost 
and discounted total utility of patients who start in the state 
“Well” for both treatment scenarios. You can assume that the discount rate is 3%.

**Problem 3: Change in Outcomes (Weight 1)**. 
Estimate the change in the expected discounted cost, the expected discounted utility, 
and the expected number of strokes when the anticoagulation drug is used. 
Report the 95% confidence intervals for all your estimates.  

**Problem 4: Cost-Utility Analysis (Weight 1)**. Use a cost-utility plane to display 
the expected discounted incremental utility and cost form the anticoagulation drug. 
Report the results of your cost-utility analysis in a table. 
Make sure to include the 95% confidence intervals for all reported estimates 
(discounted cost, discounted utility, incremental discounted cost, 
incremental discounted utility and the ICER).   

**Problem 5: Cost-Benefit Analysis (Weight 1)**. 
Plot the incremental net monetary benefit curve when the anticoagulation drugs 
is used for varying values of willingness-to-pay. 
Show the 95% confidence region. 
At what level of willingness-to-pay would you recommend adopting this 
anticoagulation drug?  
