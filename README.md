Blue-Print Boshrelease
====================================================

# Overview

A Bosh release for [Blueprint service](https://github.com/SAP/service-fabrik-blueprint-service) which can be used a sample service to try service-fabrik-broker.

Idea of blue-print boshrelease is to provide a simple blueprint service that demonstrates the Bosh release, the service agent (in our case conveniently co-located with the service and the bosh release, but in your case most likely separate repositories and maybe even bosh releases if you consume a community bosh release), the deployment manifest template, and its catalog entry.

# Requirements

 - Need to have [bosh-lite](https://bosh.io/docs/bosh-lite.html) installed on your machine.

# Download and Installation

 - Install Bosh-Lite following the instructions [here](https://github.com/SAP/service-fabrik-broker#installing-bosh-lite) .
 - Deploy on Bosh-Lite :
   
   ```
   $ git clone https://github.com/sap/service-fabrik-blueprint-boshrelease.git
   $ cd service-fabrik-blueprint-boshrelease
   $ bosh upload release
     Set the Bosh Director UUID in deployments/warden.yml
   $ bosh deployment deployments/warden.yml
   $ bosh -n deploy
   $ bosh vms
   ```

# How to Obtain Support

 If you need any support, have any question or have found a bug, please report it in the [GitHub bug tracking system](https://github.com/SAP/service-fabrik-blueprint-boshrelease/issues). We shall get back to you.


# LICENSE

This project is licensed under the Apache Software License, v. 2 except as noted otherwise in the [LICENSE](LICENSE) file
