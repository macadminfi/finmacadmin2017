# Hands on session on Zentral at FinMacAdmin 2017
Henry Stamerjohan, Apfelwerk

## Hands on Session  
Introduction to Zentral. Monitor inventory events, deploy and manage Osquery and Google Santa, integrate with Jamf Pro or Munki.

#### Idea
The idea of the hands on session is a practical Introduction to Zentral.
We start with a cloud based deployment of Zentral on AWS / Google Cloud (approx 10min). This will be followed by enrolling a macOS device and/or VM with Osquery, Santa installed to Zentral. We will explore first events in Zentral and with ElasticSearch / Kibana. (approx. 20min)

We will start importing Probes from a public feed, and create our own Probes for different event types. We will activate 3rd party integrations for JamfPro, notifications/actions like slack (or mattermost) and others.

With some time to explore on your own in your Zentral instance, we will turn into a group discussion to share knowledge, discuss scenarios. The overall idea is to gather group feedback about use cases, usability, future ideas/directions with Zentral and technologies involved.

#### Prerequisite for the workshop (mandatory) :
- Mac computer and/or a VM with current macOS (10.12, 10.11, 10.10)
- administrative rights to install software
- a public ssh key

#### Optional / additional setup (good to have):
- "readonly" account for the JSS API, in case you use JamfPro
- config/setup to manage Munki installs, in case you use Munki

#### Setup
We will use a cloud based deployment of Zentral for the workshop. To gain most from hands on training, each attendee should have access to her/his own instance of Zentral. We will provide an instance for free during the session, so everyone can participate. Of course you also can share an instance with work colleagues. This option may be "a way to go" with existing AWS/Google Cloud account, while you plan to extend using Zentral beyond the session.

For Zentral setup we plan for two variations of deployment:

A)  - *Demo instance, provided  only for the workshop *
A *Zentral-all-in-one* instance is automatically deployed and provided to you, at the beginning of the workshop. Instances will run on Google Cloud Platform and terminated after the workshop.

Although it's just a demo instance, it is critical only you have access to your personal assigned instance. To make this work, we'll need  the following from participants of this option before we start the workshop:
- SSH Public Key
- username (you want to login with via SSH)
- FQDN for the Zentral instance will be assigned to you automatically

B) - *Personal Zentral instance, controlled by you , in your own AWS or Google Cloud account*
This option is a guided deployment of Zentral with your "personal" or your "company" AWS or Google Cloud Platform account. The Instance is deployed on your own responsibility, you'll need to cover costs to run the instance as long as it's running.

- You need to have an active AWS or Google Cloud Platform account with administrator rights* - Access to setup DNS for a domain you own or control
- EC2 Instance Type *t2.medium* is required for AWS
- Machine type *1 vCPU, 3.75 GB* is required on Google Cloud Platform
- Users of GoogleCloudPlatform (GCP) should have Google Cloud SDK installed, with `gcloud` CLI tools installed and successful access the GCP services from Terminal. [https://cloud.google.com/sdk/](#)(https://cloud.google.com/sdk/)

*Tip:  Prepare for a extended trial on GoogleCloud Platform - you could  enroll for a 60 days trial + free computing budget *
Free Trial: [https://cloud.google.com/free-trial/](#)(https://cloud.google.com/free-trial/) + Google Cloud SDK [https://cloud.google.com/sdk/](#)(https://cloud.google.com/sdk/)
