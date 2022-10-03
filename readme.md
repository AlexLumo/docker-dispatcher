Cached files are located in /cache folder

To simulate activation or deletion of page you can you the following CURL commands

curl \
 -H "CQ-Action: Activate" -H "CQ-Handle: /content/test.html" \
 -H "CQ-Path: /content" -H "Content-Length: 0" \
 -H "Content-Type: application/octect-stream" \
 -H "Host: flush" http://localhost:8888/dispatcher/invalidate.cache

curl \
 -H "CQ-Action: Delete" -H "CQ-Handle: /" \
 -H "CQ-Path: /" -H "Content-Length: 0" \
 -H "Content-Type: application/octect-stream" \
 -H "Host: flush" http://localhost:8888/dispatcher/invalidate.cache
