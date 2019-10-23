### How to send a container log to Graylog

```
docker run --rm \
	--log-driver=gelf \
	--log-opt=gelf-address=tcp://graylog:12201 \
	alpine:3.9.3 \
	sh -c 'echo Hello from Alpine container'
```