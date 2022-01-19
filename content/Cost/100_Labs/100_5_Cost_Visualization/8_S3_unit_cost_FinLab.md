---
title: "View your Amazon S3 Unit Cost"
date: 2022-01-18
chapter: false
pre: "<b>8. </b>"
weight: 4
---

**NOTE**: This exercise requires you have enabled AWS Cost Explorer, this can be done by following the instructions here - [AWS Account Setup]({{< ref "100_1_AWS_Account_Setup" >}}), Step 6 - Enable Cost Explorer.

Amazon S3 Storage unit cost is a way to measure the aggregate impact of theStorage cost optimization strategies used by your Organization. Even if total S3 Storage spend is growing, a decreasing Unit Cost is a quick and simple way to communicate that optimizations have taken place and Storage spend is more efficient.

1. Click on **Cost Explorer** to go back to the default view:
![)

2. Click the **down arrow** to change the date range, select **Last 6 Months** and click **Apply**:
![)

4. Navigate to the **Group By** section and select **None**:
![)

3. Navigate to the **Filters** on the right hand side and filter **Service** to see only **S3**:
![)

4. Filter **Usage Type Group** to see anything with the prefix of **S3:Storage**:
![)

4. Filter **Charge Type** to only see **Usage**:
![)

5. Click the **Download CSV** button below the graph:
![)

6. Once downloaded, open the file in a **Spreadsheet editor**:
![)

7. **Add a column** to the right of the data in the first empty column and label it **S3 Unit Cost**:
![)

8. In that column, add the equation of **Total Cost / Total usage (GB-Month)** and apply to all rows with data:
![)

5. You will now have a monthly report of your Amazon S3 Unit Cost over the last 6 months. 
![)

{{< prev_next_button link_prev_url="../3_sp_coverage/" link_next_url="../5_ri_coverage/" />}}