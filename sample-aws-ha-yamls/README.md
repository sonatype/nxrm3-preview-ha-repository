Copyright Sonatype, Inc., 2022, All Rights Reserved.

# Overview
You can use the sample YAML files in this section to help set up the YAMLs you will need for a High-Availability (HA) Nexus Repository deployment. 
Ensure you have filled out the YAML files with appropriate information for your deployment.

> **Note** The YAML files in this section are just examples and cannot be copy-pasted and used as-is. You must fill them out with the appropriate information for your deployment to be able to use them.

# YAML Order

1. [Namespaces YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-namespaces.yaml)

2. [Storage Class YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-storage-class.yaml)

3. [Secrets YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-secrets.yaml)

4. [Fluent-bit YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-fluent-bit.yaml) (only required if using CloudWatch)

5. [Logback Tasklogfile Override YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-nxrm-logback-tasklogfile-override.yaml)

6. [Services YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-services.yaml)
   * Optional - [Ingress for Docker YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/ha-preview/sample-aws-ha-yamls/aws-ha-ingress-for-docker-connector.yaml)
   * Optional - [Nodeport for Docker YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-docker-services.yaml)

7. [Ingress YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-ingress.yaml)

8. [Service Accounts YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-service-accounts.yaml)

9. [StatefulSet YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/sample-aws-ha-yamls/aws-ha-statefulset.yaml)

> **Note** The resources created by these YAMLs are not in the default namespace.
