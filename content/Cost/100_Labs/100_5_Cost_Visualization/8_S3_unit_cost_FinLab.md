---
title: "View your Amazon S3 Unit Cost"
date: 2022-01-18
chapter: false
pre: "<b>8. </b>"
weight: 8
---

**NOTE**: This exercise requires you have enabled AWS Cost Explorer, this can be done by following the instructions here - [AWS Account Setup]({{< ref "100_1_AWS_Account_Setup" >}}), Step 6 - Enable Cost Explorer.

Amazon S3 Storage unit cost is a way to measure the aggregate impact of theStorage cost optimization strategies used by your Organization. Even if total S3 Storage spend is growing, a decreasing Unit Cost is a quick and simple way to communicate that optimizations have taken place and Storage spend is more efficient.

1. Click on **Cost Explorer** to go back to the default view:
![Images/Picture1](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture1.png)

2. Click the **down arrow** to change the date range, select **Last 6 Months** and click **Apply**:
![Images/Picture2](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture2.png)

3. Click the **down arrow** to change the interval, select **Monthly** and click **Apply**:
![Images/Picture3](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture3.png)

3. Navigate to the **Group By** section and select **None**:
![Images/Picture4](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture4.png)

4. Navigate to the **Filters** on the right hand side and filter **Service** to see only **S3** click **Apply filters**:
![Images/Picture5](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture5.png)

5. Filter **Usage Type Group** to see anything with the prefix of **S3:Storage** click **Apply filters**:
![Images/Picture6](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture6.png)

6. Click on More filters, Filter **Charge Type** to only see **Usage** click **Apply filters**:
![Images/Picture7](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture7.png)

7. Click the **Download CSV** button below the graph:
![Images/Picture8](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture8.png)

8. Once downloaded, open the file in a **Spreadsheet editor**:

9. **Add a column** to the right of the data in the first empty column and label it **S3 Unit Cost**:
![Images/Picture11](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture11.png)

10. In that column, add the equation of **Total Cost / Total usage (GB-Month)** and apply to all rows with data:
![Images/Picture10](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture10.png)

11. You will now have a monthly report of your Amazon S3 Unit Cost over the last 6 months. 

{{< prev_next_button link_prev_url="../3_sp_coverage/" link_next_url="../5_ri_coverage/" />}}