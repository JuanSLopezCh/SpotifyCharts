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
