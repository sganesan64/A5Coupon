# Required Assignment 5.1: Will the Customer Accept the Coupon? 
## Data used in this research is from the UCI Machine Learning Repository and was collected via a survey on Amazon Mechanical Turk
Please use the following link to view my findings and supporting plots created using above mentioned data : <url>https://github.com/sganesan64/A5Coupon/blob/main/PracticalAssignment1.ipynb</url>
###Problem Statement
  Identifying the most probale reason fir a customer to accept the Coupons
  
## Verified data when <u>customers accepted</u> coupons using Seaborns Joint plot correlation to the temperature and Direction
sns.jointplot(dfcpn.query("Y == 1"),x='direction_same',y='temperature',kind='kde')
 
<table><tr><td>
    <u>Fig 1:Accepted againt Direction vs temperature</u></td><td></u>Fig 2:Not Accepted againt Direction vs temperature</u>  </td></tr>
<tr><td><img width="300" height="300"  alt="Seaborn jointplot againt temperature vs accepted" src="https://github.com/user-attachments/assets/2ab2c99b-57ce-4528-ac8e-d03916893edb" /></td> <td> <img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/3a30b9f6-663d-4954-966c-f223a89277bd" />
    </td></tr></table>

## Findings 1: 
From the above plot (Fig 1) it is obvious higher temperature has positive impact on the decision to accept the coupon.

At the same time, whether same direction or not, the plot suggest that Direction has no bearing on accepting the coupon.
## Findings 2:
From the fig 2 which is plotted from the customers not accepted coupon , identified that data is not confirming that above Findings 1 is true.

### Data conditions and concerns
The percentage of customers accepted the coupon is little over 56% and not accepted is little over 43% , Meaning both cases are equally represented with the sampled population. So it might be hard to come to a conclusion based on the findings.

Cleaned data to have numbers for Text columns of Coupon by mapping numbers to categories and cleaning up age by replacing text parts

## Findings 3: After trying several plots and combinations , settled with the joint plot with Histogram. This plot prominently brought out the "Bar" coupons being brodly accepted by all age group, but not lot in the age group compared to "Coffee House" coupons###

<img width="785" height="790" alt="image" src="https://github.com/user-attachments/assets/f7036255-3067-4839-b034-d1f824fb9074" />



