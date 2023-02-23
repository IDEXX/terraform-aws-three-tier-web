# PROVIDER - MODULE NAME

**[GitHub Actions](https://github.com/idexx-labs/REPO_NAME/actions):**

![Kitchen Tests](https://github.com/idexx-labs/template-terraform-module/workflows/Kitchen%20Tests/badge.svg)

**[Bridgecrew](https://www.bridgecrew.cloud/projects?types=Passed&repository=idexx-labs%2FREPO_NAME&branch=main):**

[![Infrastructure Tests](https://www.bridgecrew.cloud/badges/github/idexx-labs/REPO_NAME/cis_PROVIDER)](https://www.bridgecrew.cloud/link/badge?vcs=github&fullRepo=idexx-labs%2FREPO_NAME&benchmark=CIS+PROVIDER+V1.1)

This module handles.... Fill in with content describing what the module does.

## Usage

**IMPORTANT:** We do not pin modules to versions in our documentation examples because of the difficulty of keeping the versions in sync with the latest released versions. We highly recommend pinning a version in your root module so that your infrastructure remains stable.

You can check the [test/fixtures](test/fixtures/) directory for example configurations. These fixtures set up the system for the testing process by providing it with all the necessary code to initialize it, thus creating good example to base your configurations on.

```hcl
module "my-module" {
  source  = "git@github.com:idexx-labs/template-terraform-module.git?ref=v0.0.0"

  foo = "bar"
  bar = "foo"
}
```

## Terraform Documentation

A child module automatically inherits default (un-aliased) provider configurations from its parent. The provider versions below are informational only and do **not** need to align with the provider configurations from its parent.

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
### Providers

No providers.

### Resources

No resources.

### Inputs

No inputs.

### Outputs

No outputs.
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->

## Module Development

See the documentation for setting up a local development environment [here](https://docs.idexx-ops.com/infrastructure_as_code/terraform/prerequisites).

Tools in use:

- [checkov](https://github.com/bridgecrewio/checkov)
- [chef-inspec](https://github.com/inspec/inspec)
- [infracost](https://github.com/infracost/infracost)
- [inspec-aws](https://github.com/inspec/inspec-aws)
- [inspec-azure](https://github.com/inspec/inspec-azure)
- [inspec-gcp](https://github.com/inspec/inspec-gcp)
- [kitchen-terraform](https://github.com/newcontext-oss/kitchen-terraform)
- [pre-commit](https://github.com/pre-commit/pre-commit)
- [pre-commit-terraform](https://github.com/antonbabenko/pre-commit-terraform)
- [terraform-docs](https://github.com/terraform-docs/terraform-docs)

### Tests

```none
bundle exec kitchen converge
bundle exec kitchen verify
bundle exec kitchen destroy
```
