<!--

    Sonatype Nexus (TM) Open Source Version
    Copyright (c) 2008-present Sonatype, Inc.
    All rights reserved. Includes the third-party code listed at http://links.sonatype.com/products/nexus/oss/attributions.

    This program and the accompanying materials are made available under the terms of the Eclipse Public License Version 1.0,
    which accompanies this distribution and is available at http://www.eclipse.org/legal/epl-v10.html.

    Sonatype Nexus (TM) Professional Version is available from Sonatype, Inc. "Sonatype" and "Sonatype Nexus" are trademarks
    of Sonatype, Inc. Apache Maven is a trademark of the Apache Software Foundation. M2eclipse is a trademark of the
    Eclipse Foundation. All other trademarks are the property of their respective owners.

-->

# Nexus Repository 3 High Availability (HA) Preview Helm and Sample YAML Repository
This repository contains resources for those in our Nexus Repository 3 High Availability Preview Program.

## Helm Chart for an HA Nexus Repository Deployment in AWS 
We provide a [Helm chart for those deploying to an AWS environment](https://github.com/sonatype/nxrm3-preview-ha-repository/tree/main/nxrm-aws-resiliency).

## Sample YAML Files for an HA Nexus Repository Deployment On Premises
You can use the sample YAML files in the [Sample YAML Files](https://github.com/sonatype/nxrm3-preview-ha-repository/tree/main/on-prem-resiliency-yamls) to help set up the YAMLs you will need for an on-premises Nexus Repository HA deployment. 

Ensure you have filled out the YAML files with appropriate information for your deployment.

> **Note** The YAML files in this section are just examples and cannot be copy-pasted and used as-is. You must fill them out with the appropriate information for your deployment to be able to use them.

## Format Limitations
For this preview program, HA supports Maven, Docker, and npm formats; once HA is available generally, it will support all formats that PostgreSQL supports
