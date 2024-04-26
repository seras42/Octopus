
By default, Nabu will construct a File based blockstore

If you are configuring a brand new Nabu instance without any data, you can enable S3 by passing in a command line parameter:
```
-s3.datastore "{\"region\": \"us-east-1\", \"bucket\": \"$bucketname\", \"rootDirectory\": \"$bucketsubdirectory\", \"regionEndpoint\": \"us-east-1.linodeobjects.com\", \"accessKey\": \"1\", \"secretKey\": \"2\"}
```
Note: accessKey and secretKey are optional. They can be set via env vars AWS_ACCESS_KEY_ID & AWS_SECRET_ACCESS_KEY or read from ~/.aws/credentials
