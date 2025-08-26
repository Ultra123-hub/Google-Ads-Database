# Google-Ads-Database
Google is a multinational technology company offering online advertising services through the Google Ads platform. As a data analyst, you have been tasked with developing a comprehensive Relational Database Management System (RDBMS) to support Google Ads operations.The goal is to manage advertisers, campaigns, ads, keywords, and performance metrics.

## Objectives
* Identifying the main entities in the database system.
* Clearly defining the attributes, relationships and constraints that support the business needs.
* Designing an entity relationship diagram that supports the business needs based on the database entities, relationships and
participation constraints.


## Main Entities in the Database
Entities are tables or real world objects that are meant to store information in a database. They are the foundational components of an Entity Relationship Diagram (ERD). 

## Advertiser
This is the table that stores the advertisers' information. The attributes and data types are as follows: <br>

AdvertiserID **INT**  PK  <br> 
AdvertiserName  **VARCHAR** <br>
ContactPerson **VARCHAR** <br>
ContactEmail  **VARCHAR** <br>

## Campaign
This is the table that stores information from the campaigns. The attributes and data types are as follows: <br>

CampaignID **INT** PK <br>
AdvertiserID **INT**  FK <br>
CampaignName **INT** <br>
StartDate **INT** <br>
Budget **INT** <br>

## Ad

AdID **INT** PK <br>
CampaignID  FK **INT** <br>
AdTitle **TEXT** <br>
TargetURL **TEXT** <br>
Impressions **INT** <br>

## Keyword
KeywordID **INT** PK <br>
AdID **INT**  FK <br>
KeywordText **TEXT** <br>
BidAmount **INT** <br>
QualityScore **INT** <br>

## Performance

PerformanceID **INT** PK  <br>
AdID **INT**  FK <br>
Date **DATE** <br>
Clicks **INT** <br>
Conversions **INT** <br>


## The Cardinality and Relationship Requirements for the Database
Advertiser - Campaign: One advertiser can manage multiple campaigns, but each campaign belongs to a single advertiser.  (one-to-many)
Campaign – Ad: One campaign can contain multiple ads, but each ad is linked to one campaign.  (one-to-many)
Ad - Keyword: An ad can target multiple keywords, but each keyword is associated with one ad.  (one-to-many)
Ad - Performance: One ad can generate multiple performance records over time, but each performance record belongs to a specific ad. (one-to-many)


## The Entity Relationship Diagram
The Entity Relationship Diagram shows the collection of objects within a database and the relationships between them. It included the entities, attributes, schemas, participation constraints and the relationships between the entities. I modelled this using the ERD tool in MySQL by adding tables, defining columns and specifying the relationships between the tables
using pre-existing columns as foreign keys.






