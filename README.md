blue-print boshrelease
====================================================

A Bosh release for Blueprint service which can be used a sample service to try service-fabrik-broker.

# Deploy on Bosh-Lite -

1. git clone https://github.com/sap/service-fabrik-blueprint-boshrelease.git
2. cd postgresql-boshrelease
3. $ bosh upload release
4. Set the Bosh Director UUID in deployments/warden.yml
5. Set deployment
   $ bosh deployment deployments/warden.yml
6. $ bosh -n deploy
7. Check $ bosh vms

## LICENSE

This project is licensed under the Apache Software License, v. 2 except as noted otherwise in the [LICENSE](LICENSE) file
