# quickstart-atlassian-confluence
## Confluence Data Center on the AWS Cloud

Use this Quick Start to deploy Confluence Data Center on the AWS Cloud.

Confluence is team collaboration software that changes how modern teams work. Confluence Data Center is a self-managed solution that gives you high availability, performance at scale, and disaster recovery for uninterrupted access to Confluence for all your teams.

This Quick Start uses the [Atlassian Standard Infrastructure (ASI)](https://fwd.aws/xYyYy) as a foundation. You can choose to build a new ASI for your deployment or deploy Confluence into your existing ASI. You can also deploy Jira and Bitbucket Data Center within the same ASI.

![Quick Start architecture for Confluence on AWS](https://d0.awsstatic.com/partner-network/QuickStart/datasheets/confluence-on-aws-architecture.png)

This Quick Start supports the use of either Amazon Relational Database Service (Amazon RDS) for PostgreSQL, which is the default, or Amazon Aurora PostgreSQL. For architectural details, best practices, step-by-step instructions, and customization options, see the [deployment guide](https://fwd.aws/kBpWN).

### Network prerequisites

You need to create the required AWS networking infrastructure
(VPC, subnets) by using the [ASI Quick Start](https://fwd.aws/xYyYy), or by deploying Confluence with a new ASI.
For details, see the [deployment guide](https://fwd.aws/kBpWN).

## Development notes

### Pre-commit hook

It is recommended that you install the hooks under `submodules/quickstart-atlassian-services/scripts/hooks/`; this will
ensure that the metadata tags in the templates are automatically updated on
commit. The simplest method of doing this is:

    git config --add core.hooksPath submodules/quickstart-atlassian-services/scripts/hooks/

Alternatively you can invoke
`submodules/quickstart-atlassian-services/scripts/hooks/update-tags.py`
manually.

## Atlassian support

This Quick Start's CloudFormation templates were developed by Atlassian, in collaboration with AWS. To report an issue or request a feature, you can [contact Atlassian directly](https://support.atlassian.com/contact/#/).

For additional Atlassian documentation on how to manage Quick Start deployments, see [Running Confluence Data Center in AWS](https://confluence.atlassian.com/x/dRBzN).
