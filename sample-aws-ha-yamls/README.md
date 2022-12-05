Copyright Sonatype, Inc., 2022, All Rights Reserved.

# Overview
You can use the sample YAML files in this section to help set up the YAMLs you will need for a High-Availability (HA) Nexus Repository deployment. 
Ensure you have filled out the YAML files with appropriate information for your deployment.

> **Note** The YAML files in this section are just examples and cannot be copy-pasted and used as-is. You must fill them out with the appropriate information for your deployment to be able to use them.

# Create Namespace
Before running the YAML files in this section, you must first create a namespace. 
To create a namespace, use a command like the following with the kubectl command-line tool:
```kubectl create namespace <namespace>```

# YAML Order
After creating the namespace, **you must run your YAML files in the order below:**

1. [Storage Class YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-storage-class.yaml)

2. [Secrets YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/aws-resiliency-yamls/aws-ha-secrets.yaml)

3. [Fluent-bit YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-fluent-bit.yaml) (only required if using CloudWatch)

4. [Logback Tasklogfile Override YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-nxrm-logback-tasklogfile-override.yaml)

5. [Services YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-services.yaml)
   * Optional - [Ingress for Docker YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-ingress-for-docker-connector.yaml)
   * Optional - [Nodeport for Docker YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-nodeport-for-docker-connector.yaml)

> **Note** The resources created by these YAMLs are not in the default namespace.
