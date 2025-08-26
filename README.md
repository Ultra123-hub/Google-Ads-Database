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

AdvertiserID **INT**   <br> 
AdvertiserName  **VARCHAR** <br>
ContactPerson **VARCHAR** <br>
ContactEmail  **VARCHAR** <br>

## Campaign
This is the table that stores information from the campaigns. The attributes and data types are as follows: <br>

CampaignID **INT** <br>
AdvertiserID **INT** <br>
CampaignName **INT** <br>
StartDate **INT** <br>
Budget **INT** <br>

## Ad

AdID **INT** <br>
CampaignID **INT** <br>
AdTitle **TEXT** <br>
TargetURL **TEXT** <br>
Impressions **INT** <br>

## Keyword
KeywordID **INT** <br>
AdID **INT** <br>
KeywordText **TEXT** <br>
BidAmount **INT** <br>
QualityScore **INT** <br>

## Performance

PerformanceID **INT** <br>
AdID **INT** <br>
Date **DATE** <br>
Clicks **INT** <br>
Conversions **INT** <br>



