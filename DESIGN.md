# Design Notes

## Overall design

* This all should run in its own namespace for easy disposal
  * default name of namespace: `kronophage`
* This should be deployable **easily**
  * User should not have to git clone anything
  * User should either type a command in the OpenShift Web Terminal, or copy paste some YAML into the OpenShift Console
* Logging
  * Logs should contain clear timestamped activities
* Service Accounts
  * used to grant pods/jobs the necessary rights
  *
* UI
  * secondary goal.


## Details

OSE (`oc`) client image:
<https://catalog.redhat.com/software/containers/openshift4/ose-cli/5cd9ba3f5a13467289f4d51d>