# File scriber based on Fluent

A file scriber based on Fluent. A file server with http plugin is required.

## Usage 

Set configuration
```
.env

TARGET_FILE_PATH=${PWD}/tracelog/                           # the log where you want to send
POS_JSON_FILE=/var/log/td-agent/fluent.metadata.json.pos    # the metadata you should set for the source
POS_ERR_FILE=/var/log/td-agent/fluent.metadata.err.pos
SOURCE_TAG=testing.tracing                                  # tag for source
HTTP_LOG_SERVER=http://localhost:16001/test.tracing         # http log server
```

Start the scriber

```bash
docker-compose up -d
```
