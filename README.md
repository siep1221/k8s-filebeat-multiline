## k8s-filebeat-multiline
multiline used in filebeat configuration

## log example:
```
^2019-12-21 | [2010-12-21] | 172.16.12.21 xxx
\t or [[:space:]] xxx
\t or [[:space:]] xxx
...
```

## pattern:
```
multiline.pattern: '^\[|^[0-9]{4}-[0-9]{2}-[0-9]{2}|^[0-9]{1,3}\.[0-9]{1,3}'
multiline.negate: true
multiline.match: after
multiline.timeout: 15s
```

## url:
```
https://www.elastic.co/guide/en/beats/filebeat/current/configuration-filebeat-options.html#_configuration_options
https://www.elastic.co/guide/en/beats/filebeat/current/filebeat-input-docker.html#filebeat-input-docker-exclude-files
```
