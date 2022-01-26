---
title: "View your Compute Savings Plan Coverage"
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
This hands-on lab will guide you through how to report on your organization's Compute or EC2 Instance Savings Plan coverage. Savings Plan coverage measures what proportion of your total Compute spend and usage is covered by your Savings Plan commitment. 

## What You Will Learn:
- How to pull Cost Explorer Reports
- How to report on Savigns Plan coverage
- What optimization opportunities there are for increasing your Savings Plan coverage

## Prerequisites: 
This exercise requires you have enabled AWS Cost Explorer, this can be done by following the instructions here - [AWS Account Setup]({{< ref "100_1_AWS_Account_Setup" >}}), Step 6 - Enable Cost Explorer.

## Steps: 

1. Click on **Cost Explorer** to get to the default view:
![Images/Picture1](/Cost/100_Savings_Plan_and_Reserved_Instance_Coverage_FinLab/Images/Picture1.png)

2. Under the **Savings Plan** section, choose **Coverage Report**:
![Images/Picture2](/Cost/100_Savings_Plan_and_Reserved_Instance_Coverage_FinLab/Images/Picture2.png)

3. Click the **Down Arrow** to change the date range to **Last 6 Months**:
![Images/Picture3](/Cost/100_Savings_Plan_and_Reserved_Instance_Coverage_FinLab/Images/Picture3.png)

4. Click on the **Down Arrow** to change the interval to **Monthly**:
![Images/Picture4](/Cost/100_Savings_Plan_and_Reserved_Instance_Coverage_FinLab/Images/Picture4.png)

5. Click the **Download CSV** button below the graph:
![Images/Picture5](/Cost/100_Savings_Plan_and_Reserved_Instance_Coverage_FinLab/Images/Picture5.png)

6. Once downloaded, open the file in a **Spreadsheet editor**


7. You will now have a monthly report of your Savings Plan and/or Reserved Instance Coverage over the last 6 months. 

8. What does this data mean? 
- If your Savings Plan coverage has **increased** from the prior month, this is a good thing! It means that more of your Compute usage is being charged at a Savings Plan rate. The Savings Plan rate will be lower than On-Demand, because in exchange for committing to a future amount of spend you receive a discount on all usage that commitment is applied to. 
- If your Savings plan coverage has **decreased** from the prior month, this is an opportunity to investigate the causes. Potential causes include growth in your On-Demand usage relative to your existing Savings Plan commitments, or changes in the underlying usage profile of your Compute such as the Instance Type or Region. 




{{< prev_next_button link_prev_url="../3_sp_coverage/" link_next_url="../5_ri_coverage/" />}}