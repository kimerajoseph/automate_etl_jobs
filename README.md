
![logo_ironhack_blue 7](https://marvel-b1-cdn.bc0a.com/f00000000243109/1x5o5mujiug388ttap1p8s17-wpengine.netdna-ssl.com/wp-content/uploads/2020/12/AWS-logo-2-400x300.jpg)
# PROJECT | AUTOMATE ETL JOBS ON AWS
## Trigger a Glue crawler and Glue ETL job every time a file is uploaded in an S3 bucket including SNS email notifications
### Intoduction
Alot of times, data engineering teams spend a considerable amount of time on routine and repeatitive tasks. In this project, we are attempting to remedy this
We set up Glue crawlers that run every time a file is added to a given S3 bucket. The crawler crawls and adds the new file/data to the Meta data catalogue. We create
new tables or append to exiting ones and make the data available for querrying with Athena and Redshift spectrum
We also run a Glue Extrat-Transform-Load (ETL) in Glue studio to clean the data before uploading it into data catalog tables

## AWS Services used
1. S3
2. Glue
3. Simple Notification Services (SNS)
4. EventBridge
5. Lambda
6. Athena

## Improvements
1. Set the S3 path dynamically so that crawler only goes through the folder where the new folder is instead of crawling the entire bucket
2. Include crawler name in the EventsBridge rules
3. Improve the formart of the message to SNS from Lambda

