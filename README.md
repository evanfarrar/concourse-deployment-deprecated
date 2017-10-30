# concourse-deployment
An IaaS agnostic general purpose concourse manifest leveraging BOSH 2.0 features

## Pre-requisites
  * [bosh bootloader](https://github.com/cloudfoundry/bosh-bootloader])
  * A director created with bbl + loadbalancers created by bbl
  * A stemcell on that director

## Usage

```
bosh deploy concourse-deployment.yml \
  -d concourse \
  --vars-store concourse-vars.yml \
  -v 'system_domain=concourse.example.com'
```
