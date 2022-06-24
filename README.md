# Blueprint Boshrelease

## Overview

A Bosh release for [Blueprint service](https://github.com/cloudfoundry/service-fabrik-blueprint-service) which can be used a sample service to try [service-fabrik-broker](https://github.com/cloudfoundry/service-fabrik-broker).

Idea of blue-print boshrelease is to provide a simple blueprint service that demonstrates the Bosh release, the service agent (in our case conveniently co-located with the service and the bosh release, but in your case most likely separate repositories and maybe even bosh releases if you consume a community bosh release), the deployment manifest template, and its catalog entry.

## Requirements

 Need to have [bosh-lite](https://bosh.io/docs/bosh-lite.html) installed on your machine.

## Download and Installation

 - Install Bosh-Lite following the instructions [here](https://bosh.io/docs/bosh-lite/#install) .
 - Deploy on Bosh-Lite :
   
   ```
   $ git clone https://github.com/cloudfoundry/service-fabrik-blueprint-boshrelease
   $ cd service-fabrik-blueprint-boshrelease
   $ bosh upload release $(ls -1rv releases/blueprint/blueprint-*.yml | head -1)
     Set the Bosh Director UUID in deployments/warden.yml
   $ bosh deployment deployments/warden.yml
   $ bosh -n deploy
   $ bosh vms
   ```

## How to Obtain Support

 If you need any support, have any question or have found a bug, please report it in the [GitHub bug tracking system](https://github.com/cloudfoundry/service-fabrik-blueprint-boshrelease/issues). We shall get back to you.


## LICENSE

This project is licensed under the Apache Software License, v. 2 except as noted otherwise in the [LICENSE](LICENSE) file
