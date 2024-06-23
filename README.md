# Sales-Dashboard

### Dashboard Link  https://app.powerbi.com/reportEmbed?reportId=6f5a3db7-3e1d-4ba6-9293-b0d78fdd4e82&autoAuth=true&ctid=66d6f9ff-29db-45b3-a345-57e9de559e0c
## Problem Statement

In this project, I developed a robust mechanism to load sales data from multiple files into a single Sales fact table, ensuring resilience against file removals and additions. This involved integrating data from diverse sources including Excel, CSV, and databases for Sales, Categories, Geography, Product, SalesRep, and SubCategories. I performed necessary transformations on the Sales fact table, such as splitting the "Location" field into "Country" and "City" columns and standardizing data types for geo-mapping.

I created unique keys (GeoKey) in both the Sales and Geography tables to ensure seamless integration and accuracy. Additionally, I developed a reusable function to clean ID columns in the SalesRep and SubCategory tables. The data model was meticulously structured, connecting all tables and incorporating a pre-existing Calendar table.

Using DAX, I calculated Total Revenue, Total Cost, and Gross Profit in the Sales table, and devised measures for Gross Profit MoM Growth, Average Sales per Day, and QoQ Growth for thorough time-based analysis. These calculations and measures were then utilized to design an intuitive, one-page sales dashboard with various visuals, effectively highlighting sales insights and trends. The dashboard also included a properly sorted month-on-x-axis feature for clear monthly analysis.

### Steps followed 

- Step 1 :Gathered requirement data from the client which he provided in a BRD and FRD file 
- Step 2 : Collected the data from various locations such as various folders, csv files and one from a SQL server
- Step 3 : Modelled the data accordingly connect important tables with each other on the basis of foreign key and primary keys, in this project there were several many to many and some single to many models 
- Step 4 : Cleaned the modelled data and formatted them accordingly cleaned various columns as they had duplicate data some column headers were missing, some had aggregated values, cleaned and formatted them accordingly.
- Step 5 : Started Ui creation in the BI desktop version ,had to create various measure such as MOM growth, YOY growth, Gross profit% etc 
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Additional calculations were done using DAX formulae 
- Step 8 : Visual filters (Slicers) were added for four fields named "Year", "Country", "Month Name" & "Type of travel".
- Step 9 : Added various cards like "Sumoftotalrevenue", "sumofgrossprofit", "sumofunits", "Sumofrevenuebycategory" all of them are reactive based on the slicers .
           Using visual level filter from the filters pane, basic filtering was used & null values were unselected for consideration into average calculation.
           USed Futher aftermarket visuals as scrollers for interactive dashboard visuals 
           
           Although, by default, while calculating average, blank values are ignored.
- Step 10 :  Published the powerbi desktop file to powerBi service account and did various level of RLS, created a dashboard in teh service pannel and lastly created an app for seamless sharing in between organisational users 

In our dataset, Some parameters were assigned value 0, representing those parameters are not applicable for some products.

All these values have been ignored while calculating average rating for each of the parameters mentioned above.

An Imgae of the slicers that ive created for seamless transition in between data 
![image](https://github.com/asjadbaig-boop/salesdashboard/assets/63597780/17ad8b19-ab24-4445-a555-27e13949c27f)


The scroller that ive downloaded for displaying important datas 
![image](https://github.com/asjadbaig-boop/salesdashboard/assets/63597780/7ae6f982-7f27-44f0-826a-8dc095de3b76)


Cards that i created for Focus on major KPIs
![image](https://github.com/asjadbaig-boop/salesdashboard/assets/63597780/b255640b-7bc0-4dd0-9677-9f4da1827ecb)


Some more important pie-charts and static visuals 
![image](https://github.com/asjadbaig-boop/salesdashboard/assets/63597780/22e0a471-37ce-4aa9-aa2d-dde3f2a8715d)


Sum of revenue by product name and SubCategories
![image](https://github.com/asjadbaig-boop/salesdashboard/assets/63597780/3603fcfa-8517-4190-80e0-8cf8dff4e5ee)



Some more important visuals that the client demanded to categorize his total revenue by category, year and product name
![image](https://github.com/asjadbaig-boop/salesdashboard/assets/63597780/ff234e8a-9808-4f5f-b0cc-4fc23bbca74e)


Important complex sales data jotted in form of line graph for better understanding of the busines owner and what are the things he needs to focus more on 
![image](https://github.com/asjadbaig-boop/salesdashboard/assets/63597780/b2d4354d-c236-4885-b41d-30481119fdcc)
