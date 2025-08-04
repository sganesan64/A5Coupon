# Required Assignment 5.1: Will the Customer Accept the Coupon? 
## Data used in this research is from the UCI Machine Learning Repository and was collected via a survey on Amazon Mechanical Turk
Please use the following link to view my findings and supporting plots created using above mentioned data : <url>https://github.com/sganesan64/A5Coupon/blob/main/PracticalAssignment1.ipynb</url>
## Verified data when customers accepted coupons using Seaborns Joint plot correlation to the temperature
    sns.jointplot(dfcpn.query("Y == 1"),x='direction_same',y='temperature',kind='kde')
    <seaborn.axisgrid.JointGrid at 0x2125eefbfe0>
    <url>https://github.com/sganesan64/A5Coupon/blob/main/images/sns_joint_accepted_temp.PNG</url>