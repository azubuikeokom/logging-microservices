# Logging and monitoring microservices
The logging system design is based on the sidecar logging agent. Where the sidecar container is deployed in thesame pod as the microsevice running in a kubernetes cluster.

# Elastic search 
Auto generate password,enrollment token for elastic search
    kubectl exec -it elasticsearch -- bin/elasticsearch-reset-password -u elastic
    kubectl exec -it elasticsearch -- bin/elasticsearch-create-enrollment-token -s kibana
# Kibana
Generate kibana verification code
    kubectl exec -it kibana -- bin/kibana-verification-code


