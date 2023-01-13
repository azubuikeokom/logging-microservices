# Logging and monitoring microservices
The logging system design is based on the sidecar logging agent. Where the sidecar container is deployed in thesame pod as the microsevice running in a kubernetes cluster.

# Elastic search 
Auto generate password with the command below. Generated password will be used to authenticate to elasticsearch by the logging agent
    kubectl exec -it elasticsearch -- bin/elasticsearch-reset-password -u elastic
Auto-generate the enrollment token. This token will be used to enroll kibana to the elasticsearch backend
    kubectl exec -it elasticsearch -- bin/elasticsearch-create-enrollment-token -s kibana
# Kibana
Generate kibana verification code. Login to kibana UI with it
    kubectl exec -it kibana -- bin/kibana-verification-code


