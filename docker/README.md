Schema Registry Container for OpenShift 3
=========================================

Version of a popular Schema Registry Docker image (docker pull spec: confluentinc/cp-schema-registry)
that will run on OpenShift 3 with the default Security Context Constraint (SCC)
of restricted.

The cp-schema-registry docker image (at least version 3.3.0) runs fine under the **restricted** SCC already,
so no customization of the image is required at this time.

# Importing Docker image into OpenShift
There is a YAML file in the openshift directory (schemaregistry-imagestream.yml) which will
import the confluentinc/cp-schema-registry image(s) into the internal registry of an OpenShift
cluster.
