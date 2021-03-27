# SpringBoot2ELKExample
## ELK stack configuration
### Elasticsearch
A.	Download latest version of Elasticsearch from this download (https://www.elastic.co/downloads/elasticsearch) page and unzip it any folder. \
B.	Run bin\elasticsearch.bat from command prompt. \
C.	By default, it would start at http://localhost:9200 
### Kibana
A.	Download the latest distribution from download (https://www.elastic.co/downloads/kibana) page and unzip into any folder. \
B.	Open config/kibana.yml in an editor and set elasticsearch.hosts to point at your Elasticsearch instance. In our case as we will use the local instance just uncomment elasticsearch.hosts: "http://localhost:9200" \
C.	Run bin\kibana.bat from command prompt. \
D.	Once started successfully, Kibana will start on default port 5601 and Kibana UI will be available at http://localhost:5601 

### Logstash
A.	Download the latest distribution from download (https://www.elastic.co/downloads/logstash) page and unzip into any folder. \
B.	Create one file logstash.conf as per configuration instructions (https://www.elastic.co/guide/en/logstash/current/configuration.html). \
C.	Now run bin/logstash -f logstash.conf to start logstash 
