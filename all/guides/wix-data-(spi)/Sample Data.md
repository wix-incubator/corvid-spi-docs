SortOrder: 3
# Sample Data

The examples in the following sections are based on a MySQL database with the following tables and data:



#### Car Table
|Column Name|Data Type   |
|-----------------|------|
|_id        |varchar(36) |
|_owner|varchar(36)
|date_added| datetime|
|make| varchar(100)|
|model|varchar(100)|
|year| int|
  


#### Car Table Data

|_id |_owner |make |model|year|date_added |
|------------------------------------|------------------------------------|-------------|-------|----|---------------------|
|86cbf595-d369-48bb-8649-c6c082c003ca|81c9168e-95b8-47fd-8e6a-ad9fdf71b38e| Ford | Mustang | 1995 | 2001-06-07 21\:00\:00.0|
|95953ca3-5fe5-4ce7-9cca-9bcc1ba64ba6|81c9168e-95b8-47fd-8e6a-ad9fdf71b38e|Toyota |Corolla|2019|2020-09-30 21\:30\:00.0|
|1e68ce9c-a7bc-4440-a9d4-7ce6b42e5be8|81c9168e-95b8-47fd-8e6a-ad9fdf71b38e|Mercedes-Benz|E Coupe|2020|2020-06-16 21\:30\:00.0|
|93d1a47e-6e65-4bd1-a13d-69fbae8a9fa3|81c9168e-95b8-47fd-8e6a-ad9fdf71b38e|Citroen |C3 |1987|2020-02-13 22\:00\:00.0|
|2e3d9a71-805b-40f3-b662-902569b6f772|81c9168e-95b8-47fd-8e6a-ad9fdf71b38e|Citroen |C5 |2014|2015-03-31 21\:00\:00.0|
|6d04fb52-f317-4d7b-bc23-46dd1c74d5a8|81c9168e-95b8-47fd-8e6a-ad9fdf71b38e|Hyundai |Tuscon |2005|2020-08-31 21\:00\:00.0|
|f551864f-4022-430e-b311-0215b9c9ac38|81c9168e-95b8-47fd-8e6a-ad9fdf71b38e|Hyundai |I20 |2018|2018-07-31 21\:00\:00.0|
|295f6831-ce44-429d-aeb9-e3a91cdfc6e0|81c9168e-95b8-47fd-8e6a-ad9fdf71b38e|Nissan |Maxima |2012|2012-07-31 21\:00\:00.0|
|20cd8f8d-1a0f-4530-91df-6d31fe9e83a5|81c9168e-95b8-47fd-8e6a-ad9fdf71b38e|Ferrari |812GTS |2020|2020-03-31 21\:00\:00.0|
|9a08a341-8bdc-49e4-8cdb-280571d658d2|81c9168e-95b8-47fd-8e6a-ad9fdf71b38e|Mazda |2 |2014|2013-06-22 21\:00\:00.0|
|4b0841dc-2355-4351-9cbc-2b6c9cf53cec|81c9168e-95b8-47fd-8e6a-ad9fdf71b38e|Mazda |MX5 |2003|2002-12-09 22\:00\:00.0|



#### Manufacturer Table

|Column Name|Data Type |
|-----------------|------|
|name | varchar(100) |
|country | varchar(100) |
|established | datetime |
|_id | varchar(36)|
|_owner | varchar(36)|
|share_price | decimal(10,0) |



#### Manufacturer Table Data

|name          |country|established          |_id    |_owner|share_price|
|--------------|-------|---------------------|-------|------|-----------|
|Ford          |USA    |1903-01-01 12\:00\:00.0|abc-123|      |          6|
|Nissan        |Japan  |1933-12-06 12\:00\:00.0|abc-124|      |        412|
|Mercedes-Benz¶|Germany|1926-01-01 12\:00\:00.0|abc-125|      |        145|
|Mazda         |Japan  |1920-01-30 12\:00\:00.0|abc-126|      |        696|
|Ferrari       |Italy  |1947-01-01 12\:00\:00.0|abc-127|      |        152|
|Citroen       |France |1919-01-01 00\:00\:00.0|abc-128|      |        234|
|Hyundai       |Korea  |1967-01-01 00\:00\:00.0|abc-129|      |        741|

