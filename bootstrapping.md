# Bootstrapping an AWS Account
The bootstrap process is a required pre-condition for utilizing an AWS account for usage as a target for deployment. Essentially, it takes care of ensuring we have the prerequisites (such as terraform state storage, IAM roles, IAM policies) deployed for usage by the Nerdamigo pipeline and/or local development.

Once bootstrapped, updates/revisions to the bootstrapping version is self-referencing, and your deployment pipeline can simply take a dependency on the [terraform-aws-account-bootstrap module]()

## What is Deployed?
* IAM Role