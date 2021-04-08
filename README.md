# aws-serverless-nodejs-log-forwarder
Demo of how to ship logs from CloudWatch Logs to a Kinesis stream, and then ship them to S3 and Elasticsearch.


A group of Lambda functions for:

* shipping logs from Kinesis stream to S3
* auto-subscribe new log groups to the configured Kinesis stream so you don't have to subscribe them manually
* auto-updates the retention policy of new log groups to 7 days (configurable)