# terraform-utils

Better Terraform CLI experience with real use cases.

## Usage

First, pull the terraform state file from the remote.

```bash
terraform state pull > terraform.tfstate.json
```

Then use the `terraform.tfstate.json` as the `<state-file>` for the following use cases.

## Use cases

You can clone the repo and run scripts individually or use the following one-liners directly.

### generate terraform imports for all resources

## Usage

```bash
TF_UTIL_VERSION=1.1.0
curl -sSL "https://raw.githubusercontent.com/amazingandyyy/terraform-utils/$TF_UTIL_VERSION/terraform-imports-generate.sh" | bash -s -- <state-file> <output-file>
```

### terraform list with ids

```bash
TF_UTIL_VERSION=1.1.0
curl -sSL "https://raw.githubusercontent.com/amazingandyyy/terraform-utils/$TF_UTIL_VERSION/terraform-state-list-ids.sh" | bash -s -- <state-file>
```

## LICENSE

MIT

