---
title: "Create an AWS KMS Custom Managed Key (CMK)"
chapter: false
weight: 32
---



We have precreated a CMK key for the EKS cluster to use when encrypting your Kubernetes secrets, let's retrieve its ARN and store it as the `MASTER_ARN` environment variable and add it to our `bash_profile`
```bash
export MASTER_ARN=$(aws kms describe-key --key-id alias/eksworkshop2 --query KeyMetadata.Arn --output text)
echo "export MASTER_ARN=${MASTER_ARN}" | tee -a ~/.bash_profile
```

To test that your EKS cluster is up and running, execute
```bash
kubectl get nodes
```

You should see 3 workers with Status = Ready. This concludes the prereqs section.
