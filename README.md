# Real-Time Weather Data Pipeline (AWS + Snowflake)


This project demonstrates a **real-time, data engineering pipeline** built using AWS services and Snowflake. The pipeline continuously collects live weather data from a public Weather API, stores it in DynamoDB, streams changes to S3 and loads the data into Snowflake via Snowpipe for downstream analytics.

The goal is to showcase **event-driven architecture, real-time ingestion, cloud-native ETL and Snowflake integration** without managing servers.


##  Data Flow
Weather API → AWS Lambda → DynamoDB → DynamoDB Streams → Lambda → S3 → Snowflake → Snowflake External Table → Analytics Table


##  Testing the Pipeline
- Trigger EventBridge manually  
- Validate DynamoDB updates 
- Check S3 bucket for new JSON files  
- Verify Snowpipe loads data correctly
