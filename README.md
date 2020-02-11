# k8s-filebeat-es-logging

1. Change the ENV variables on yaml file (ELASTICSEARCH_HOST, ELASTICSEARCH_PORT, ELASTICSEARCH_USERNAME, ELASTICSEARCH_PASSWORD)In our case we are running ELK outside the k8s cluster, hence we are using IP address on environment variables
2. We are using basic authentication of ES which we have setup on ELK end using the below command
```
	/usr/share/elasticsearch/bin/elasticsearch-setup-passwords interactive

```
3. I presume these passwords will get set on bootstrap and it cannot be changed/edited/removed without re-installation.
