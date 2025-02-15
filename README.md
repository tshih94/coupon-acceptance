# Professional Certificate in Machine Learning and Artificial Intelligence
## Module 5: Practical Application 1: Will the Customer Accept the Coupon?

The data comes from the UCI Machine Learning repository and was collected through a survey from the Amazon Mechanical Turk. The original project file comes form the Professional Certificate in Machine Learning and Artificial Intelligence class offered by BerkeleyExecEd|BerkeleyHaas, where it guides students through some initial analysis on the dataset as an example before becoming an open-ended investigation for students to find their own independent conclusions. This data used is in the data folder of this repository as a [CSV file](https://github.com/tshih94/coupon-acceptance/blob/main/data/coupons.csv) here.

Link for the [The Jupyter Notebook](https://github.com/tshih94/coupon-acceptance/blob/main/prompt.ipynb)

## Findings (Guided)
The guided portion of the analysis focused on finding out what drives acceptance rates for coupons for bars, with **41%** of people offered bar coupons accepting the coupon overall. The acceptance rate jumped to **76%** when focusing only on people who reported they went to a bar 3 or more times a month compared to **37%** for those that did not go that often.

Lowering the monthly threshold to once or more a month but raising the age threshold to 25 and older yielded a **69.5%** acceptance rate, and further narrowing the criteria to those with adult passengers and were not in the forestry, farming, or fishing industries produced **71.8%**, not a meaningful difference from when focusing solely on monthly frequency of visits. Playing around with income, marital status, and monthly frequency at other businesses as guided by the instructions lowered the acceptance rate. 

In conclusion, a major difference between people who accepted a coupon for a bar and those who did not was the self-reported monthly frequency of visiting a bar. **To increase acceptance rate, the recommendation is to offer coupons to those who frequent bars. One way to do so is to advertise and offer coupons around bars.** Other characteristics to consider in further analysis are time of day, since bars typically are not open during the mornings, and breakdowns along gender.

## Findings (Independent)
For the independent analysis, I focused on Coffeehouse coupons, looking to figure out what characteristics are associated with accepting a coffeehouse coupon. For a baseline, exactly half (**50%**) those offered coffeehouse coupons accepted them. 

Since monthly frequency of visiting bars proved to be very predictive of if a person would accept a coupon for a bar, monthly frequency of visits to coffeehouses were graphed against acceptance rates, resulting in acceptance rates rising and **plateauing at 1~3 and above**. With coffee being so important for certain times of the day, graphing against time of day when the coupon was offered found a **spike in acceptance rates at 10AM in the mornings**, and doing the same against income found a **dip in the $75000 - $87499 income range**.

Combining these 3 observations, the next graph was for our "target group": people who visited coffeehouses at least once a month, were offered the coupon at 10am, and were NOT in the $75000 - $87499 income range.
The graph, images/target_group.png, found that **81%** of them accepted coupons for coffeehouses versus only **46%** for datapoints that did not fit into the target group.

Finally, while a combination of characteristics have been found that indicate high coffeehouse coupon acceptance rate, businesses are always looking to gain loyal, lifelong customers. Graphing the target group (images/target_group_and_age.png) against age reveals that young people, 21 and below to 21 accept coffee coupons at a high rate regardless of whether they are in the target group or not. However, as age goes up, the target group acceptance rate remains high while non-target group acceptance drops off. 

This indicates an opportunity for coffeehouses to market to young people and offer them coupons, which they accept at high rates regardless, to get them going to coffeehouses more often, moving them from the infrequent drinkers group (blue) into the frequent drinker group (orange), turning them into lifelong drinkers of coffee whose rates of continuing to drink coffee and accepting more coffeehouse coupons do not drop as they age.

In conclusion, to have high coffeehouse coupon acceptance rates, and thus to make the best use of time giving out coupons, **the recommendation is to give them out at 10am, give them to all young people** in hopes of ~~hooking them on caffeine~~ building a habit of drinking coffee and going to coffeehouses. Should this be accomplished, they may remain loyal coffee drinkers into old age, as indicated by images/target_group_and_age.png chart. 

Similarly, just like with bars, offer coffeehouse coupons to frequent visitors of coffeehouses, as the data shows they accept coupons for coffeehouses at a very high rate. **Again, advertise and offer coupons around coffeehouses to more frequently encounter those who frequent coffeehouses.** Further analysis might look into the distance to the advertised coffeehouse and see if there is a drop off in coupon acceptance for coffeehouses farther away, not to mention how people might be in more of a hurry in the mornings.


## Built With
* [Jupyter Notebooks](https://jupyter.org/) - Python3

## Authors

* **Tinyen Shih** 

## Acknowledgments
This project was created as a class assignment for the class Professional Certificate in Machine Learning and Artificial Intelligence, part of the Emeritus program from:
* [BerkeleyExecEd|BerkeleyHaas](https://em-executive.berkeley.edu/)
* [UCI Machine Learning repository, data from Amazon Mechanical Turk]