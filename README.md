# ceu_product-analytics

The project involves answering questions around Product analytics topics such as Acquisition, Activity and Retention.
Done as a requisite of the Mastering Product Analytics course at Central European University in Hungary. Medium.com article can be found on https://medium.com/@bencetth/product-analytics-65812e82b2c2

## Datasets

* Based on a real SaaS product subsampled and simplified for the task 

* Two datasets 

  * *registrations.csv*: unique users with basic demographics
  
  * *activity.csv*: which users have been active in which month
  
**Registration data**

* Columns

  * *id*: unique identifier of a registered user(e.g id_5)
  
  * *registration_month*: number of the month from 1 to 21 
  
    * Month1 and Month13 are both January in consecutive years
    
    * No need to deal with date type
    
  * *region*: America, EMEA, or ROW (every other country)
  
  * *operating_system*: Windows, Mac, Linux, Unknown
  
* About 40K records
  
* Each record is a unique registered user
  
**Activity data**

* Columns

  * *id*: unique identifier of a registered user(e.g id_5)
  
  * *activity_month*: number of the month from 1 to 21
  
    * Month1 and Month13 are both January in consecutive years
    
    * No need to deal with date type
    
  * Additional Columns:
  
    * Registration data joined to the activity records as convenience
  
* About 79K activity events
  
  * One record represents an active user in a specific month
    
  * It means a user is active in two months on average (long tail distribution)
