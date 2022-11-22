Copyright Sonatype, Inc., 2022, All Rights Reserved.

# Overview
You can use the sample YAML files in this section to help set up the YAMLs you will need for a high-availability (HA) Nexus Repository deployment. 
Ensure you have filled out the YAML files with appropriate information for your deployment.

> **Note** The YAML files in this section are just examples and cannot be copy-pasted and used as-is. You must fill them out with the appropriate information for your deployment to be able to use them.

# Create Namespace
Before running the YAML files in this section, you must first create a namespace. 
To create a namespace, use a command like the following with the kubectl command-line tool:
```kubectl create namespace <namespace>``` 

# YAML Order
After creating the namespace, **you must run your YAML files in the order below:**
1. [Persistent Volume YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/on-prem-ha-yamls/on-prem-ha-nfs-persistent-volume.yaml)
2. [Persistent Volume Claim YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/on-prem-ha-yamls/on-prem-ha-nfs-persistent-volume-claim.yaml)
3. [License Configuration Mapping YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/on-prem-ha-yamls/on-prem-ha-license-config-mapping.yaml)
4. [Deployment YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/on-prem-ha-yamls/on-prem-ha-deployment.yaml)
5. [Services YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/on-prem-ha-yamls/on-prem-ha-services.yaml)
   * Optional - [Ingress for Docker YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/on-prem-ha-yamls/on-prem-ha-ingress-for-docker-connector.yaml)
   * Optional - [Nodeport for Docker YAML](https://github.com/sonatype/nxrm3-preview-ha-repository/blob/main/on-prem-ha-yamls/on-prem-ha-nodeport-for-docker-connector.yaml)
   
> **Note** The resources created by these YAMLs are not in the default namespace.
