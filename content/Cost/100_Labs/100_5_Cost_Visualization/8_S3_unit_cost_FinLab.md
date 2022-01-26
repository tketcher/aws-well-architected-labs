---
title: "View your Amazon S3 Unit Cost"
date: 2022-01-18
chapter: false
pre: "<b>8. </b>"
weight: 8
---
## Authors
- Lauren Mytnik, Commercial Architect, OPTICS, AWS
- Tony Weldon, Impact Computing Program Manager, AWS

## Feedback
If you wish to provide feedback on this lab, there is an error, or you want to make a suggestion, please email: costoptimization@amazon.com

## Introduction
This hands-on lab will guide you through how to report on your organization's Amazon S3 Storage unit cost. Amazon S3 Storage unit cost is a way to measure the aggregate impact of the Storage cost optimization strategies used by your Organization. Even if total S3 Storage spend is growing, a decreasing Unit Cost is a quick and simple way to communicate that optimizations have taken place and Storage spend is more efficient.

## What You Will Learn:
- How to pull Cost Explorer Reports
- How to report on Amazon S3 Unit Cost
- What optmization opportunities there are for Amazon S3

## Prerequisites: 
This exercise requires you have enabled AWS Cost Explorer, this can be done by following the instructions here - [AWS Account Setup]({{< ref "100_1_AWS_Account_Setup" >}}), Step 6 - Enable Cost Explorer.

## Steps:

1. Click on **Cost Explorer** to navigate to the default view:
![Images/Picture1](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture1.png)

2. Click the **down arrow** to change the date range, select **Last 6 Months** and click **Apply**:
![Images/Picture2](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture2.png)

3. Click the **down arrow** to change the interval, select **Monthly** and click **Apply**:
![Images/Picture3](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture3.png)

4. Navigate to the **Group By** section and select **None**:
![Images/Picture4](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture4.png)

5. Navigate to the **Filters** on the right hand side and filter **Service** to see only **S3** click **Apply filters**:
![Images/Picture5](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture5.png)

6. Filter **Usage Type Group** to see anything with the prefix of **S3:Storage** click **Apply filters**:
![Images/Picture6](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture6.png)

7. Click on More filters, Filter **Charge Type** to only see **Usage** click **Apply filters**:
![Images/Picture7](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture7.png)

8. Click the **Download CSV** button below the graph:
![Images/Picture8](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture8.png)

9. Once downloaded, open the file in a **Spreadsheet editor**:

10. **Add a column** to the right of the data in the first empty column and label it **S3 Unit Cost**:
![Images/Picture11](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture11.png)

11. In that column, add the equation of **Total Cost / Total usage (GB-Month)** and apply to all rows with data:
![Images/Picture10](/Cost/100_Amazon_S3_Unit_Cost_FinLab/Images/Picture10.png)

12. You will now have a monthly report of your Amazon S3 Unit Cost over the last 6 months. 

13. What does this data mean? 
- If your S3 unit cost has **decreased** from last month, this is good! This means that on average, every unit of storage (measured as Gigabytes of data), was cheaper than it was in the prior month. It can be the result of using a service like S3 Intelligent-tiering to migrate infrequently accessed data to lower cost S3 storage tiers, or migrating that data manually. 
- If your S3 unit cost has **increased** from last month, this is an opportunity to investigate the causes. A potential cause can be increasing use of S3 Standard Storage (the most expensive storage tier) relative to cheapertiers such as Infrequent-Access and Glacier. 

{{< prev_next_button link_prev_url="../3_sp_coverage/" link_next_url="../5_ri_coverage/" />}}