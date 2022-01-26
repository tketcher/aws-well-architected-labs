---
title: "View your Compute Savings Plan Utilization"
date: 2022-01-18
chapter: false
pre: "<b>9. </b>"
weight: 9
---
## Authors
- Lauren Mytnik, Commercial Architect, OPTICS, AWS
- Tony Weldon, Impact Computing Program Manager, AWS

## Feedback
If you wish to provide feedback on this lab, there is an error, or you want to make a suggestion, please email: costoptimization@amazon.com

## Introduction
This hands-on lab will guide you through how to report on your organization's Compute or EC2 Instance Savings Plan utilization. Savings Plan Utilization measures how much of your Savings Plan commitment purchase has been applied to instances (used), as a percentage of the total cost of the Savings Plan. Regularly reporting on and assessing your organization's Savings Plan utilization can help to ensure that you are getting the most out of your investment. 

## What Will You Learn:
- How to pull Cost Explorer Reports
- How to report on Savings Plan Utilization
- What optimization opportunities there are for increasing your Savings Plan Utilization

## Prerequisites:
This exercise requires you have enabled AWS Cost Explorer, this can be done by following the instructions here - [AWS Account Setup]({{< ref "100_1_AWS_Account_Setup" >}}), Step 6 - Enable Cost Explorer.

## Steps: 

1. Click on **Cost Explorer** to get to the default view:
![Images/Picture1](/Cost/100_Savings_Plan_and_Reserved_Instance_Utilization_FinLab/Images/Picture1.png)

2. Under the **Savings Plan** or **Reserved Instance** section, choose **Utilization Report**:
![Images/Picture2](/Cost/100_Savings_Plan_and_Reserved_Instance_Utilization_FinLab/Images/Picture2.png)

3. Click the **Down Arrow** to change the date range to **Last 6 Months**:
![Images/Picture3](/Cost/100_Savings_Plan_and_Reserved_Instance_Utilization_FinLab/Images/Picture3.png)

4. Click on the **Down Arrow** to change the interval to **Monthly**:
![Images/Picture4](/Cost/100_Savings_Plan_and_Reserved_Instance_Utilization_FinLab/Images/Picture4.png)

5. Click the **Download CSV** button below the graph:
![Images/Picture5](/Cost/100_Savings_Plan_and_Reserved_Instance_Utilization_FinLab/Images/Picture5.png)

6. Once downloaded, open the file in a **Spreadsheet editor**

7. You will now have a monthly report of your Savings Plan and/or Reserved Instance Utilization over the last 6 months. 

8. What does this data mean? 
- If your Savings Plan utilization has **increased** from the prior month, this is a good thing! It means that that your commitment is being applied to more of the usage in your account. 
- If your Savings Plan utilization has **decreased** from the prior month, this is an opportunity to investigate possible causes. It could mean that you've committed to a usage profile (Instance Family, Region) that isn't being applied to existing usage in your account. 

{{< prev_next_button link_prev_url="../3_sp_coverage/" link_next_url="../5_ri_coverage/" />}}