## Awesome CloudFormation

A curated list of resources for working with AWS CloudFormation.

## License Summary

This sample code is made available under a modified MIT license. See the LICENSE file.

## Linting

All templates should pass linting by the [CloudFormation Linter](https://github.com/aws-cloudformation/cfn-python-lint):

```console
$ cfn-lint "**/*.yaml"
```

If you'd like cfn-lint to be run automatically when making changes to files in your Git repository, you can install [pre-commit](https://pre-commit.com/). This repo includes the necessary `.pre-commit-config.yaml` file to perform this and other linting automatically. The same linting will also be run against pull requests, so installing the pre-commit hooks with `pre-commit install` saves a bit of time.

Here are some formatting guidelines for consistency:

* YAML files are strongly preferred (with the file ending `*.yaml`), because they allow comments
* Use the short form of functions (`!Ref logicalName` instead of `Ref: logicalName`, or even `{"Ref": "logicalName"}`). This makes some of the more complex functions easier to read
* Indentation: two spaces, to match the existing AWS Documentation

The pre-commit hooks/CI will also check for other common text issues, such as trailing whitespace, UTF-8 byte-order marks (BOM), and a lack of newlines/too many newlines at the end of files.
