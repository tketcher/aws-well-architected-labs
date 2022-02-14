---
title: "View your EC2-Instance Savings Plan Coverage"
date: 2022-01-18
chapter: false
pre: "<b>10. </b>"
weight: 10
---
## Authors
- Lauren Mytnik, Commercial Architect, OPTICS, AWS
- Tony Weldon, Impact Computing Program Manager, AWS

## Feedback
If you wish to provide feedback on this lab, there is an error, or you want to make a suggestion, please email: costoptimization@amazon.com

## Introduction
This hands-on lab will guide you through how to report on your organization's EC2 Instance Savings Plan coverage. Savings Plan coverage measures what proportion of your total EC2-Instance spend and usage is covered by your Savings Plan commitment. 

## What You Will Learn:
- How to pull Cost Explorer Reports
- How to report on Savigns Plan coverage
- What optimization opportunities there are for increasing your Savings Plan coverage

## Prerequisites: 
This exercise requires you have enabled AWS Cost Explorer, this can be done by following the instructions here - [AWS Account Setup]({{< ref "100_1_AWS_Account_Setup" >}}), Step 6 - Enable Cost Explorer.

## Steps: 

1. Click on **Cost Explorer** to get to the default view:
![Images/SavingsPlanCoverage1.png](/Cost/100_5_Cost_Visualization/Images/SavingsPlanCoverage1.png?classes=lab_picture_small)

2. Under the **Savings Plan** section, choose **Coverage Report**:
![Images/SavingsPlanCoverage2.png](/Cost/100_5_Cost_Visualization/Images/SavingsPlanCoverage2.png?classes=lab_picture_small)

3. Click the **Down Arrow** to change the date range to **Last 6 Months**:
![Images/SavingsPlanCoverage3.png](/Cost/100_5_Cost_Visualization/Images/SavingsPlanCoverage3.png?classes=lab_picture_small)

4. Click on the **Down Arrow** to change the interval to **Monthly**:
![Images/SavingsPlanCoverage4.png](/Cost/100_5_Cost_Visualization/Images/SavingsPlanCoverage4.png?classes=lab_picture_small)

5. Navigate to the filters section. Under Service choose **EC2-Instances** only and click apply filters:
![Images/SavingsPlanCoverage6.png](/Cost/100_5_Cost_Visualization/Images/SavingsPlanCoverage6.png?classes=lab_picture_small)

6. Click the **Download CSV** button below the graph:
![Images/SavingsPlanCoverage5.png](/Cost/100_5_Cost_Visualization/Images/SavingsPlanCoverage5.png?classes=lab_picture_small)

7. Once downloaded, open the file in a **Spreadsheet editor**

8. You will now have a monthly report of your EC2-Instance Savings Plan Coverage over the last 6 months. 

9. What does this data mean? 
- If your Savings Plan coverage has **increased** from the prior month, this is a good thing! It means that more of your Compute usage is being charged at a Savings Plan rate. The Savings Plan rate will be lower than On-Demand, because in exchange for committing to a future amount of spend you receive a discount on all usage that commitment is applied to. If your coverage is at 100%, it is possible that you have over-committed which can result in waste.   
- If your Savings plan coverage has **decreased** from the prior month, this is an opportunity to investigate the causes. Potential causes include growth in your On-Demand usage relative to your existing Savings Plan commitments, or changes in the underlying usage profile of your Compute such as the Instance Type or Region. 


Note: You can do the same steps for Reserved Instances. In step 2, You will navigate to the Reserved Instance section. Follow steps 3 and 4 from above. Then in step 5 filter to your desired service. 

{{< prev_next_button link_prev_url="../3_sp_coverage/" link_next_url="../5_ri_coverage/" />}}