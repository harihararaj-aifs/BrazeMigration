# Acoustic Data Architecture

## Databases (Master Database)
Stores core **contact profiles** such as unique ID, name, email, phone, and other attributes.  
This is the **primary source of truth** for identifying and targeting users across all campaigns.

## Relational Tables
Store **transactional, behavioral, or additional profile data** (e.g., purchases, loyalty info, activity logs).  
They can be linked to the Master Database to create **1:1 or 1:many** relationships for deeper segmentation and personalization.

## Suppression Lists
Hold contacts who should **not receive emails**.  
- **Database Suppression List:** Opt-outs only for a specific database.  
- **Global Suppression List:** Org-wide opt-outs from *all* campaigns.  
These lists protect sender reputation and ensure compliance. There can also be a supression list for the mailing

## Contact Lists
Static or imported lists used for **targeted mailings**. Helpful for uploading external segments or running specific campaigns without altering the master database.

## Subscription Groups
Represent **email preference categories** (e.g., Newsletter, Promotions, Alerts).  
Allow contacts to opt out **per category** instead of unsubscribing from all messages.

## Test / Seed Lists
Internal lists included in test sends or used to consistently send campaign copies to stakeholders, ensuring **quality checks** before or during live sends.
