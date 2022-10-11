# USWDS Starter for SF Projects

This is a demonstration repo to show the folder structure needed to compile

## Prerequisites

- Node
- SFDX CLI

## Instructions

Compile resources into assets/uswds/ directory.

`npx gulp compile`

## Creating Zip File for StaticResource

```sh
zip -r uswds_3_x.zip assets/uswds/css/*.css* scss/ assets/uswds/fonts/*/*.ttf assets/uswds/fonts/*/*.woff assets/uswds/img/ assets/uswds/js/*.min.js*
```

Upload resulting .zip into Salesforce Static Resources, overwriting previous versions.

| Field         | Pattern                                                | Example                                                                         |
| ------------- | ------------------------------------------------------ | ------------------------------------------------------------------------------- |
| Name          | {filename without .zip}                                | uswds_3_x                                                                       |
| Description   | uswds {full version number}<br>{link to USWDS version} | uswds v3.1.0<br>CSS Files<br>https://github.com/uswds/uswds/releases/tag/v3.1.0 |
| Cache Control | n/a                                                    | Public                                                                          |

# Salesforce DX Project: Next Steps

Now that you’ve created a Salesforce DX project, what’s next? Here are some documentation resources to get you started.

## How Do You Plan to Deploy Your Changes?

Do you want to deploy a set of changes, or create a self-contained application? Choose a [development model](https://developer.salesforce.com/tools/vscode/en/user-guide/development-models).

## Configure Your Salesforce DX Project

The `sfdx-project.json` file contains useful configuration information for your project. See [Salesforce DX Project Configuration](https://developer.salesforce.com/docs/atlas.en-us.sfdx_dev.meta/sfdx_dev/sfdx_dev_ws_config.htm) in the _Salesforce DX Developer Guide_ for details about this file.

## Read All About It

- [Salesforce Extensions Documentation](https://developer.salesforce.com/tools/vscode/)
- [Salesforce CLI Setup Guide](https://developer.salesforce.com/docs/atlas.en-us.sfdx_setup.meta/sfdx_setup/sfdx_setup_intro.htm)
- [Salesforce DX Developer Guide](https://developer.salesforce.com/docs/atlas.en-us.sfdx_dev.meta/sfdx_dev/sfdx_dev_intro.htm)
- [Salesforce CLI Command Reference](https://developer.salesforce.com/docs/atlas.en-us.sfdx_cli_reference.meta/sfdx_cli_reference/cli_reference.htm)
