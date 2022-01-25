---
title: "View your Commitment Utilization"
date: 2022-01-18
chapter: false
pre: "<b>9. </b>"
weight: 9
---

**NOTE**: This exercise requires you have enabled AWS Cost Explorer, this can be done by following the instructions here - [AWS Account Setup]({{< ref "100_1_AWS_Account_Setup" >}}), Step 6 - Enable Cost Explorer.

EC2 Savings Plan and Reserved Instance Utilization measures how much of your Savings Plan commitment or Reserved Instance purchase has been applied to instances (used), as a percentage of the total cost of the Savings Plan or Reserved Instance.

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

{{< prev_next_button link_prev_url="../3_sp_coverage/" link_next_url="../5_ri_coverage/" />}}