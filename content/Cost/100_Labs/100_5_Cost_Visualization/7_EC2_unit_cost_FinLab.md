---
title: "View your Amazon EC2 Unit Cost"
date: 2022-01-18
chapter: false
pre: "<b>7. </b>"
weight: 7
---
## Authors
- Lauren Mytnik, Commercial Architect, OPTICS, AWS
- Tony Weldon, Impact Computing Program Manager, AWS

## Feedback
If you wish to provide feedback on this lab, there is an error, or you want to make a suggestion, please email: costoptimization@amazon.com

## Introduction
This hands-on lab will guide you through how to report on your organization's Amazon EC2 unit cost. The average cost per Amazon EC2 usage hour, also known as the EC2 unit cost, is a great way to measure the aggregate impact of the EC2 cost optimization strategies used by your Organization. Even if total EC2 spend is growing, a decreasing EC2 Unit Cost is a quick and simple way to communicate that optimizations have taken place and EC2 spend is more efficient. 

## What You Will Learn:
- How to pull reports from Cost Explorer
- How to report on meaningful EC2 Unit Cost metrics
- What optmization opportunities there are for EC2

## Prerequisites: 
This exercise requires you have enabled AWS Cost Explorer, this can be done by following the instructions here - [AWS Account Setup]({{< ref "100_1_AWS_Account_Setup" >}}), Step 6 - Enable Cost Explorer.

## Steps:

1. Click on **Cost Explorer** to navigate to the default view:
![Images/EC2UnitCost1.png](/Cost/100_5_Cost_Visualization/Images/EC2UnitCost1.png?classes=lab_picture_small)

2. Click the **down arrow** to change the date range, select **Last 6 Months** and click **Apply**:
![Images/EC2UnitCost2.png](/Cost/100_5_Cost_Visualization/Images/EC2UnitCost2.png?classes=lab_picture_small)

3. Click the **down arrow** to change the interval, select **Monthly** and click **Apply**:
![Images/EC2UnitCost3.png](/Cost/100_5_Cost_Visualization/Images/EC2UnitCost3.png?classes=lab_picture_small)

4. Navigate to the **Group By** section and select **Service**:
![Images/EC2UnitCost4.png](/Cost/100_5_Cost_Visualization/Images/EC2UnitCost4.png?classes=lab_picture_small)

5. Navigate to the **Filters** on the right hand side and filter in the **Usage Type Group** to see only **EC2 Running Hours**:
![Images/EC2UnitCost5.png](/Cost/100_5_Cost_Visualization/Images/EC2UnitCost5.png?classes=lab_picture_small)

6. Navigate to the **Advanced Options** section underneath the filters and select **Show Cost as: Amortized**:
![Images/EC2UnitCost6.png](/Cost/100_5_Cost_Visualization/Images/EC2UnitCost6.png?classes=lab_picture_small)

7. Click the **Download CSV** button below the graph:
![Images/EC2UnitCost7.png](/Cost/100_5_Cost_Visualization/Images/EC2UnitCost7.png?classes=lab_picture_small)

8. Once downloaded, open the file in a **Spreadsheet editor**

9. **Add a column** to the right of the data in the first empty column and label it **EC2 Unit Cost**:
![Images/EC2UnitCost8.png](/Cost/100_5_Cost_Visualization/Images/EC2UnitCost8.png?classes=lab_picture_small)

10. In Column F, add the equation of **Total Cost / Total usage (Hrs)** and apply to all rows with data:
![Images/EC2UnitCost9.png](/Cost/100_5_Cost_Visualization/Images/EC2UnitCost9.png?classes=lab_picture_small)

11. You will now have a monthly report of your Amazon EC2 Unit Cost over the last 6 months. 

12. What does this data mean? 
- If your EC2 unit cost has **decreased**, this is good! This means that, on average, each EC2 instance hour you ran was cheaper than it was the prior month. It can be the result of committing to a new pricing model like a Savings Plan, utilizing Spot Instances, or replacing existing usage with lower cost alternatives (rightsizing). 
- If your EC2 unit cost has **increased** from last month, this is an opportunity to investigate the causes. Potential causes can be the utilization of a new instance type, or the expriation of a Savings Plan that previously covered EC2 usage in your account. You can use Cost Explorer to dive deeper into your cost and usage, and understand how trends have changed. 

{{< prev_next_button link_prev_url="../3_sp_coverage/" link_next_url="../5_ri_coverage/" />}}