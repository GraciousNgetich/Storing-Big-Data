# Storing-Big-Data

<div align="center">
  <img src="https://github.com/GraciousNgetich/Storing-Big-Data/blob/main/on-premise.png" width="900" height="400"/>
</div>

This project is divided into two major parts:
### Establishing an On-Premise Source Connection - This enables organizations to capture data in real-time or near-real-time from their on-premise sources and store it in the cloud.

Services I Used:
 1. Aws IAM to manage roles and permissions
 2. Cloud Formation to provision the infrastructure
 3. File Gateway, and NFS File share for seamless data transfer from cloud to on-premise
 4. Cloud Watch Alarms which will trigger when a data transfer over a specified threshold is exceeded.

### Streaming data 

Services I used
 1. DynamoDB as a mock data streaming source
 2. Lambda Script to run and generate new data that can simulate a data stream.
 3. Lambda trigger to automate the process attached to an SNS topic for lambda alert failure
 4. AWS Kinesis Firehorse to receive a stream of data and to place this into S3-based object storage.
