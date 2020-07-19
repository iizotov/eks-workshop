---
title: "Your environment"
chapter: false
weight: 14
---

-
{{% notice info %}}
This workshop was designed to run in the **Oregon (us-west-2)** region. **Please don't
run in any other region.**
{{% /notice %}}


{{% notice tip %}}
Ad blockers, javascript disablers, and tracking blockers should be disabled for
the cloud9 domain, or connecting to the workspace might be impacted.
Cloud9 requires third-party-cookies. You can whitelist the [specific domains]( https://docs.aws.amazon.com/cloud9/latest/user-guide/troubleshooting.html#troubleshooting-env-loading).
{{% /notice %}}

### Your environment:

Because you're attending a formal AWS event today, we bootstrapped your AWS account by preprovisioning the following services to save time:

* EKS Cluster: [eksworkshop-eksctl](https://us-east-2.console.aws.amazon.com/eks/home?region=us-east-2#/clusters)
  * in your spare time, feel free to [research](/beginner-optional/030_eksctl/) about the `eksctl` utility we used to set up the cluster
* Cloud9 Workspace: [EKS-Workshop-IDE](https://us-east-2.console.aws.amazon.com/cloud9/home?region=us-east-2). In your Cloud9 environment we set up a few things for you:
  * cloned these repositories under `~/envoronment`:
  ```
  git clone https://github.com/brentley/ecsdemo-frontend.git
  git clone https://github.com/brentley/ecsdemo-nodejs.git
  git clone https://github.com/brentley/ecsdemo-crystal.git
  ```
  * installed `awscli`, `kubectl` and a couple of more command-line utilities

* a couple of IAM roles and a KMS Customer Managed Key

Before we proceed, we need you to log into you Cloud9 Workspace and update its IAM setting: [Update IAM settings for your Workspace](/020_prerequisites/workspaceiam/)




