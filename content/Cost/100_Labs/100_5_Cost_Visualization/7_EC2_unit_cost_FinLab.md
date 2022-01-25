---
title: "View your Amazon EC2 Unit Cost"
date: 2022-01-18
chapter: false
pre: "<b>7. </b>"
weight: 7
---

**NOTE**: This exercise requires you have enabled AWS Cost Explorer, this can be done by following the instructions here - [AWS Account Setup]({{< ref "100_1_AWS_Account_Setup" >}}), Step 6 - Enable Cost Explorer.

The average cost per EC2 usage hour, also known as the EC2 unit cost, is a great way to measure the aggregate impact of the EC2 cost optimization strategies used by your Organization. Even if total EC2 spend is growing, a decreasing EC2 Unit Cost is a quick and simple way to communicate that optimizations have taken place and EC2 spend is more efficient.

1. Click on **Cost Explorer** to go back to the default view:
![Images/Picture1](/Cost/100_Amazon_EC2_Unit_Cost_FinLab/Images/Picture1.png)

2. Click the **down arrow** to change the date range, select **Last 6 Months** and click **Apply**:
![Images/Picture2](/Cost/100_Amazon_EC2_Unit_Cost_FinLab/Images/Picture2.png)

3. Click the **down arrow** to change the interval, select **Monthly** and click **Apply**:
![Images/Picture3](/Cost/100_Amazon_EC2_Unit_Cost_FinLab/Images/Picture3.png)

4. Navigate to the **Group By** section and select **Service**:
![Images/Picture4](/Cost/100_Amazon_EC2_Unit_Cost_FinLab/Images/Picture4.png)

5. Navigate to the **Filters** on the right hand side and filter in the **Usage Type Group** to see only **EC2 Running Hours**:
![Images/Picture5](/Cost/100_Amazon_EC2_Unit_Cost_FinLab/Images/Picture5.png)

6. Navigate to the **Advanced Options** section underneath the filters and select **Show Cost as: Amortized**:
![Images/Picture6](/Cost/100_Amazon_EC2_Unit_Cost_FinLab/Images/Picture6.png)

7. Click the **Download CSV** button below the graph:
![Images/Picture7](/Cost/100_Amazon_EC2_Unit_Cost_FinLab/Images/Picture7.png)

8. Once downloaded, open the file in a **Spreadsheet editor**

9. **Add a column** to the right of the data in the first empty column and label it **EC2 Unit Cost**:
![Images/Picture8](/Cost/100_Amazon_EC2_Unit_Cost_FinLab/Images/Picture8.png)

10. In Column F, add the equation of **Total Cost / Total usage (Hrs)** and apply to all rows with data:
![Images/Picture9](/Cost/100_Amazon_EC2_Unit_Cost_FinLab/Images/Picture9.png)

11. You will now have a monthly report of your Amazon EC2 Unit Cost over the last 6 months. 

{{< prev_next_button link_prev_url="../3_sp_coverage/" link_next_url="../5_ri_coverage/" />}}