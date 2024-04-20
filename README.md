# Spotify Charts Analysis
![Spo_charts Logo](https://charts.spotify.com/SpotifyChartsLogoPurple.svg)



Welcome to the Top 200 Global Chart Automation project! 🎶

This project automates the process of downloading the top 200 global chart from Spotify every week using Selenium. The retrieved data is then added to an Azure SQL database, where it can be accessed and analyzed. Finally, the data is visualized in a Power BI file for comprehensive analysis and insights.

## Key Features:
**Automation:** Weekly retrieval of the top 200 global chart from Spotify using Selenium.<br>
**Data Storage:** Storing the downloaded data in an Azure SQL database for easy access and management.<br>
**Visualization:** Creating visualizations and insights using Power BI for deeper analysis of the global music trends.<br>
**Scalability:** Easily customizable and scalable to accommodate additional features or modifications.<br>


## Creating the Azure SQL Database

For this project, I utilized the free 32GB Azure account available to set up the necessary infrastructure, including an Azure SQL Database server.

### Steps Taken:
**Azure Portal:** I accessed the Azure Portal and signed in with my Azure account credentials.<br>
**Creating a New SQL Database Server:** Within the Azure Portal, I navigated to the "Create a resource" section and searched for "SQL Database". From there, I selected the option to create a new SQL Database.<br>
**Configuring the Server:** During the creation process, I specified the details for the SQL Database server, including the server name, resource group, location, and server admin credentials.<br>
**Selecting the Pricing Tier:** As part of the setup, I opted for the free tier, which offers 32GB of storage and 5 DTU (Database Transaction Units) of performance, suitable for small-scale projects and testing purposes.<br>
**Setting Firewall Rules:** To ensure secure access to the database, I configured firewall rules to allow access from specific IP addresses or ranges. This helps protect the database from unauthorized access.<br>
**Deployment Completion:** After reviewing the configuration settings, I initiated the deployment process and waited for Azure to provision the SQL Database server.<br>
**Connection String:** Once the deployment was complete, I obtained the connection string for the SQL Database server, which includes the server name, database name, and authentication credentials. This connection string is used by the scripts to establish a connection to the database and perform operations such as data insertion and retrieval.

### Benefits:
**Cost-Efficiency:** Leveraging the free tier of Azure SQL Database allowed me to create a cost-efficient solution for storing and managing the project's data without incurring additional expenses.<br>
**Scalability:** While the free tier provides ample resources for small-scale projects, Azure SQL Database offers scalability options to accommodate growth as the project evolves.<br>

**Reliability:** Azure SQL Database provides high availability and data redundancy features to ensure the reliability and durability of the stored data.<br>
By leveraging Azure SQL Database, I was able to create a robust and reliable data storage solution for the Top 200 Global Chart Automation project, enabling seamless data management and analysis.

## Automation Process
Every Friday, a Selenium Python script is automated using the Windows Task Scheduler to download and update the server. This ensures that the latest data from the Top 200 Global Chart is fetched and stored in the Azure SQL Database, ready for analysis in the Power BI file.

### Steps Involved:
**Selenium Script Execution:** A Python script leveraging Selenium is scheduled to run every Friday using the Windows Task Scheduler. This script automates the process of accessing the Spotify website, downloading the Top 200 Global Chart data, and saving it locally.<br>
**Updating the Server:** Once the data is downloaded, the script updates the Azure SQL Database server with the latest information. This ensures that the database remains up-to-date with the most recent music trends.<br>
**Power BI File Update:** After the server is updated, the Power BI file is automatically refreshed to reflect the changes in the dataset. This ensures that the visualizations and insights provided in the Power BI file are always based on the latest data.

### Benefits:
**Efficiency:** Automating the data retrieval and update process saves time and effort by eliminating the need for manual intervention.<br>
**Consistency:** By scheduling the script to run at regular intervals, we ensure that the database and Power BI file are consistently updated with the latest information.<br>
**Timeliness:** Having the data updated every Friday ensures that analysts and stakeholders have access to the most recent insights for informed decision-making.


By automating the process using the Windows Task Scheduler, we maintain a seamless and efficient workflow for keeping our data and analysis up-to-date.
