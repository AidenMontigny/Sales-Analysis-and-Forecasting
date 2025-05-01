<h1> Sales Analysis and Forecasting </h1>

<h2>Description</h2>
This project involves the development of queries to analyze sales data for 'Mountain King' footwear in the Chicagoland region, specifically focusing on sales during the 1st and 2nd quarters of 2024. The insights derived from these queries are critical for informing key business decisions. By examining detailed sales patterns, businesses can optimize inventory management to ensure high-demand products are adequately stocked. Additionally, the analysis supports targeted marketing efforts, allowing companies to refine advertising strategies for maximum engagement and impact. Evaluating vendor performance, customer preferences, and regional dynamics provides a comprehensive understanding of the business landscape, guiding inventory procurement, vendor relationships, and regional marketing initiatives. Moreover, leveraging historical sales data for forecasting enhances the accuracy of demand predictions, enabling businesses to allocate resources effectively and minimize potential revenue loss. Ultimately, these queries enable decision-makers to make data-driven choices, fostering strategic growth and improving competitiveness in the market.
<br />

<h2>Languages and Utilities Used</h2>

- <b> Powershell </b> 
- <b> Command Prompt </b>
- <b> Active Directory Users and Computers </b>
- <b> Group Policy Managment Console </b>
- <b> Windows Server Manager </b>
- <b> DNS Manager </b>

<h2>Environments Used </h2>

- <b> Windows Server 2019 </b>

<h2>Project walk-through:</h2>
<p align="left">
The CalendarDimension table is designed to store comprehensive date-related information, including <br/> a unique CalendarKey, full date, day of the week, day of the month, month, quarter, <br/> and year, enabling efficient time-based analysis and reporting. <br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
 The `StoreDimension` table is designed to store essential store-related information, including a <br/> unique `StoreKey`, store identifier (`StoreID`), store zip code (`StoreZip`), and region  <br/> identifier (`RegionID`), facilitating detailed store-level analysis and reporting. <br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
The `ProductDimension` table is designed to store detailed product information, including a unique <br/> `ProductKey`, product identifier (`ProductID`), product name (`ProductName`), product price <br/> (`ProductPrice`), vendor identifier (`VendorID`), and category identifier (`CategoryID`), enabling <br/> efficient product-level analysis and reporting.<br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
The `CustomerDimension` table is designed to store key customer information, including a unique <br/> `CustomerKey`, customer identifier (`CustomerID`), customer name (`CustomerName`), and customer <br/> zip code (`CustomerZip`), supporting detailed customer-level analysis and reporting. <br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
The `RegionDimension` table is designed to store region-specific information, including a unique <br/> `RegionID` and the corresponding `RegionName`, enabling region-based analysis and reporting. <br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
 The `SalesFact` table is designed to store transactional sales data, including a unique `SalesID`,<br/> references to the `CalendarKey`, `StoreKey`, and `ProductKey` from the respective dimension <br/> tables, along with `DollarsSold` and `UnitsSold` values, enabling detailed sales analysis and <br/> reporting across time, store, and product dimensions.<br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
This query retrieves all columns from the `CalendarDimension` table, showing date-related details like <br/> `CalendarKey`, `FullDate`, `DayofWeek`, `DayofMonth`, `Month`, `Quarter`, and `Year`, with <br/> results for January 1st and 2nd, 2024. <br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
 This query retrieves all columns from the `ProductDimension` table, showing product details like  <br/> `ProductKey`, `ProductID`, `ProductName`, `ProductPrice`, `VendorID`, and `CategoryID` for various  <br/> products. <br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
This query retrieves all columns from the `CustomerDimension` table, displaying customer details such <br/> as `CustomerKey`, `CustomerID`, `CustomerName`, and `CustomerZip` for various customers. <br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
This query retrieves all columns from the `RegionDimension` table, showing region details such as <br/>`RegionID` and `RegionName`, with entries for "Chicagoland" and "Tristate". <br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
<p align="left">
This query retrieves sales data from the `SalesFact` table, joined with `ProductDimension` and <br/> `CalendarDimension`, filtering for sales on Wednesdays in the first two quarters of 2024 for 'FW' products <br/> from the 'MK' vendor in the 'Chicagoland' region. The result shows sales details, including product names <br/> and dates, for "Zzz Bag" and "Easy Boot" sold on January 1st, 2024. <br/><br/>
  <img src="Screenshot 2025-04-17 202325.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br/>
