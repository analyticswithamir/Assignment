# Power-BI-Assignment-2

### 1. Explain the advantages of Natural Queries in PowerBi with an example?

- It requires no prior knowledge on any querying language like SQL, excel. Querying is carried out using common and natual English language.
- Once dashboard is created and submitted to Business stakeholders, stakeholders find it easy to query on their own in the report submitted by the Analyst Team.
- Power BI shows predictions as user types the query which indeed helps user to query faster and confidently
- It reduces confusion to layman

for example, we may query **"show total sales country wise"**. Power BI understands the query as we type. When we type "show" it lists all the features available. The respected query results are displayed to user/Business stakeholders.

![image](https://user-images.githubusercontent.com/89411580/149671834-d714b9d1-f431-49c6-88a5-84fa33f96143.png)


### 2. Explain Web Front End(WFE) cluster from Power BI Service Architecture?

Power BI service Architecture contains two clusters.
- Web Front End cluster (WFE)
- Back end cluster

Web Front End(WFE) cluster manages two important components.
- Initial connection
- User Autentication

Frond end cluster acts as intermediary between client and back end. 

It uses **Azure Traffic Manager (ATM)** to make efficient and quick authentication. It attemps to send user traffic to nearest data center to reduce connection time. The nearest location is found by the DNS record of client attempting to connect.

Once user is connected, he/she can access static content & files. To share these files, Power BI uses another technology called **Azure Content Delivery(ACD)** to efficiently distribute the respective user file contents based on geographic locale.

Power BI uses **Azure Active Directory (AAD)** to authenticate users who sign in to the Power BI service, and in turn, uses the Power BI login credentials whenever a user attempts to access resources that require authentication

![image](https://user-images.githubusercontent.com/89411580/149663992-184dafb2-638e-4758-a78e-9f18bc047f67.png)


### 3. Explain Back End cluster from Power BI Service Architecture?

The Power BI services at the back end take care of 
  - visualizations
  - datasets
  - storage
  - reports
  - data connections
  - data refreshing and other interactions with Power BI. 

At the back-end, a web client has only two direct points of interaction
- Azure API Management
- Gateway Role. 

The Gateway Role acts as a gateway between user requests and the Power BI service. Users do not interact directly with any roles other than the Gateway Role. Azure API Management will eventually handle the Gateway Role. Azure API Management will eventually handle the Gateway Role.

These two components are responsible for load balancing, authentication, authorization, routing, etc.

![image](https://user-images.githubusercontent.com/89411580/149664526-7354aad7-f11b-426b-a382-3455c9a3ee53.png)

### 4. What ASP.NET component does in Power BI Service Architecture?

ASP.NET is a web development platform provided by microsoft. 
- ASP ==> Active Server Page
- NET ==> Network Enabled Technologies

ASP.NET component plays a major role while publishing reports and dashboards to workspace where stakeholder interact with it in front end provided by Power BI service. Not only that, BI dashboards can also be accessed through other apps like Microsoft teams which embeds BI Applicaiton through ASP.NET framework

![image](https://user-images.githubusercontent.com/89411580/149671695-2baeb635-05c0-4c6a-b96c-3cdf47f53b40.png)


### 5. Compare Microsoft Excel and PowerBi Desktop on the following features:
### - Data import
### - Data transformation
### - Modeling
### - Reporting
### - Server Deployment
### - Convert Models
### - Cost

![image](https://user-images.githubusercontent.com/89411580/149671962-5d9764c1-8dc6-4f15-a464-76fda37c7c0c.png)


### 6. List 20 data sources supported by Power Bi desktop.

1) Access database
2) Oracle Database
3) IBM Netezza
4) Mysql Database
5) Postgre Database
6) Teradata Database
7) Amazon Redshift
8) Impala
9) Google Bin query
10) Vertica
11) Snowflake
12) Essbake
13) Azure SQL Database
14) Sharepoint Online list
15) Microsoft Exchange online
16) Dynamics 365(online)
17) Adobe Analytics
18) Github(beta)
19) Linkedin Sales Navigator(Beta)
20) Twilio(beta)

![image](https://user-images.githubusercontent.com/89411580/149668782-e2756a30-2332-4f28-971e-648367860067.png)

