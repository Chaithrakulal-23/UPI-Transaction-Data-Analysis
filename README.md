# UPI Transaction Data Analysis
### Dashboard Link : https://app.powerbi.com/links/T7QsvIhiGL?ctid=51697115-1ecd-42b5-b509-2d62c3919f76&pbi_source=linkShare&bookmarkGuid=bf1bd228-929c-41c0-bdb3-448e163df55b

## Problem Statement

This dashboard helps analyze UPI transaction data to understand user behavior, transaction trends, and financial patterns. It enables identification of peak transaction periods, performance across cities and banks, and balance trends over time.

By using this dashboard, stakeholders can monitor transaction volume, analyze usage patterns, and identify areas for improving digital payment efficiency.

### Steps followed 

 Step 1 : Loaded Excel dataset into Power BI Desktop.
 Step 2 : Opened Power Query Editor and enabled Column Distribution Column Quality Column Profile.
 Step 3 : Checked and corrected data types for all columns.
 Step 4 : Split Transaction Time column using delimiter to separate Date and Time.
 Step 5 : Removed unnecessary Date column and renamed Time column.
 Step 6 : Performed data cleaning and ensured no inconsistencies in dataset.
 Step 7 : Created a new Age Group column using DAX.

For creating new column following DAX expression was written;
       
        Age Group = 
        
      IF('UPI Transaction '[CustomerAge] <= 25, "A1", 
      IF('UPI Transaction '[CustomerAge] <= 35, "A2", "A3" ))

        
Snap of new Age Group column ,

![Snap_1](https://user-images.githubusercontent.com/102996550/174089602-ab834a6b-62ce-4b62-8922-a1d241ec240e.jpg)

 Step 8 : Added slicers for the following fields:

  - Bank Name Sent

  - Bank Name Received

  - City

  - Device Type

  - Gender

  - Age Group

  - Merchant Name

  - Purpose

  - Transaction Type
  - 
![Snap_of_Slicers](https://user-images.githubusercontent.com/102996550/174089602-ab834a6b-62ce-4b62-8922-a1d241ec240e.jpg)

Step 9 : Synced slicers across both pages using Sync Slicers.

Step 10 : Created Page 1 visuals using line and column charts to represent monthly transaction trends for 2024 and analyze balance variations over time.

Step 11 : Created Page 2 Visuals using Matrix Visual to compare monthly transaction and balance trends across cities and currencies.

Step 12 : Applied Page level filter using Currency across all pages.

Step 14 : Used Selection Pane to control visibility of visuals.

Step 15 : Implemented Bookmarks to toggle between visuals.

![Snap_of_Bookmarks](https://user-images.githubusercontent.com/102996550/174089602-ab834a6b-62ce-4b62-8922-a1d241ec240e.jpg)

Step 16 : Added Bookmark Navigator Buttons for smooth user interaction.

![Snap_of_Navigator](https://user-images.githubusercontent.com/102996550/174089602-ab834a6b-62ce-4b62-8922-a1d241ec240e.jpg)
Step 17 : Designed and finalized dashboard layout.

Step 18 : Published report to Power BI Service.
 
![Publish_Message](https://user-images.githubusercontent.com/102996550/174094520-3a845196-97e6-4d44-8760-34a64abc3e77.jpg)

 
 # Report Snapshot Page 1

 
![Dashboard_upload](https://user-images.githubusercontent.com/102996550/174074051-4f08287a-0568-4fdf-8ac9-6762e0d8fa94.jpg)

# Report Snapshot Page 2

 
![Dashboard_upload](https://user-images.githubusercontent.com/102996550/174074051-4f08287a-0568-4fdf-8ac9-6762e0d8fa94.jpg)

# Insights

[1] Transaction Trends

Identified monthly transaction patterns for 2024

Peak transaction periods observed during specific months

[2] City-wise Analysis

Certain cities contribute higher transaction volumes

Regional usage patterns indicate digital adoption differences

[3] Balance Analysis

Remaining balance trends vary across time and location

Helps understand spending behavior

[4] User Segmentation

Age group and gender-based transaction behavior identified

Device type and transaction type influence usage patterns

[5] Filtering & Interaction

Dynamic slicers allow deep analysis across multiple dimensions

Bookmark navigation improves user experience




