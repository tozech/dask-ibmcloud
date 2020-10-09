IBM Cloud
=========

Create account
--------------

* Must upgrate lite version to pay-as-you-go with credit card in order to have access to free kubernetes service.

* Follow CLI install instructs
** Install sudo apt-get install ca-certicates
** Use wget instead of curl
   wget https://ibm.biz/idt-installer
   export CURL_CA_BUNDLE=/etc/ssl/certs/ca-certificates.crt
   bash idt-installer

The following steps must be repeated each time restart shell

* Login to ibmcloud 
ibmcloud login -a cloud.ibm.com -r eu-de -g Default

* Set Kubernetes context
ibmcloud ks cluster config --cluster bu0d974f007vgi8nqq70

* Verify connection
kubectl config current-context

See more kubectl commands
https://kubectl.docs.kubernetes.io/


Took me one hour
