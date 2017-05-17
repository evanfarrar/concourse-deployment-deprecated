# concourse-deployment
An IaaS agnostic general purpose concourse manifest leveraging BOSH 2.0 features

## Pre-requisites
  * [bosh bootloader](https://github.com/cloudfoundry/bosh-bootloader])
  * A director created with bbl + loadbalancers created by bbl
  * A stemcell on that director
  
## Usage

`bosh -d concourse deploy --vars-store concourse-vars.yml concourse-deployment.yml -v 'domain=concourse.example.com'`
