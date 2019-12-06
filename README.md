## Awesome CloudFormation [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of resources and projects for working with [AWS CloudFormation](https://aws.amazon.com/cloudformation/).

## Contents

- [CloudFormation Sample Templates](#cloudformation-sample-templates)
- [Authoring & Testing Tools](#authoring--testing-tools)
- [CLI Tools](#cli-tools)
- [Code Generation](#code-generation)
- [Custom Resource Development](#custom-resource-development)
- [Public Coverage Roadmap](#public-coverage-roadmap)
- [Blog Posts & Talks](#blog-posts--talks)
- [Documentation](#documentation)

## CloudFormation Sample Templates

The following are pre-built sample templates demonstrating how to use AWS CloudFormation to construct various canned applications or resource groupings.

- [aws-cf-templates](https://github.com/widdix/aws-cf-templates): Free Templates for AWS CloudFormation
- [aws-cloudformation-templates](https://github.com/awslabs/aws-cloudformation-templates): Sample AWS CloudFormation templates which are intended to support learning how to declare specific AWS resources or solve particular use cases.
- [aws-quickstart](https://github.com/aws-quickstart): Automated gold-standard deployments on AWS
- [asecure.cloud](https://asecure.cloud/): A free repository of customizable AWS security configurations and best practices

## Authoring & Testing Tools

These tools are designed to assist in the authoring and testing process for AWS CloudFormation. Tools include template generation, linting and testing applications.

- [AWSConsoleRecorder](https://github.com/iann0036/AWSConsoleRecorder): Records actions made in the AWS Management Console and outputs the equivalent CLI/SDK commands and CloudFormation/Terraform templates.
- [Former2](https://github.com/iann0036/former2): Generate CloudFormation / Terraform / Troposphere templates from your existing AWS resource
- [cfn-python-lint](https://github.com/aws-cloudformation/cfn-python-lint): Validate CloudFormation yaml/json templates against the CloudFormation spec and additional checks. Includes checking valid values for resource properties and best practices.
- [cfn_nag](https://github.com/stelligent/cfn_nag): The cfn-nag tool looks for patterns in CloudFormation templates that may indicate insecure infrastructure.
- [taskcat](https://github.com/aws-quickstart/taskcat): taskcat is a tool that tests AWS CloudFormation templates. It deploys your AWS CloudFormation template in multiple AWS Regions and generates a report with a pass/fail grade for each region.

## CLI Tools

This section contains tools which have been designed to improve the experiene of interacting with the CloudFormation service through a terminal session.

- [awscfncli](https://github.com/Kotaimen/awscfncli): awscfncli helps build and manage complex AWS CloudFormation stacks.
- [stacker](https://github.com/cloudtools/stacker): An AWS CloudFormation Stack orchestrator/manager.
- [sceptre](https://github.com/Sceptre/sceptre): Sceptre is a tool to drive AWS CloudFormation. It automates the mundane, repetitive and error-prone tasks, enabling you to concentrate on building better infrastructure.

## Code Generation

If you prefer imperative coding, or just using your favourite programming language, the following projects are intended to abstract the creation of AWS CloudFormation templates.

- [aws-cdk](https://github.com/aws/aws-cdk): The AWS Cloud Development Kit (AWS CDK) is an open-source software development framework to define cloud infrastructure in code and provision it through AWS CloudFormation.
- [serverless-application-model](https://github.com/awslabs/serverless-application-model): The AWS Serverless Application Model (SAM) is an open-source framework for building serverless applications. It provides shorthand syntax to express functions, APIs, databases, and event source mappings. With just a few lines of configuration, you can define the application you want and model it.
- [mu](https://github.com/stelligent/mu): Similar to how the Serverless Framework improved the developer experience of Lambda and API Gateway, this tool makes it easier for developers to use EKS or ECS as a microservices platform.
- [troposphere (Python)](https://github.com/cloudtools/troposphere): The troposphere library allows for easier creation of the AWS CloudFormation JSON by writing Python code to describe the AWS resources. troposphere also includes some basic support for OpenStack resources via Heat.
- [sparkleformation (Ruby)](https://github.com/sparkleformation): A magical Ruby infrastructure orchestration DSL
- [VaporShell (PowerShell)](https://github.com/scrthq/VaporShell): A PowerShell module for building, packaging and deploying AWS CloudFormation templates.

## Custom Resource Development

When you need to extend AWS CloudFormation to support your own personal or organizational use-cases, the following tools are intended to support the development experience with the [original Custom Resources](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/template-custom-resources.html) functionality and the new [CloudFormation Registry](https://aws.amazon.com/about-aws/whats-new/2019/11/now-extend-aws-cloudformation-to-model-provision-and-manage-third-party-resources/) experience.

- [cloudformation-cli](https://github.com/aws-cloudformation/cloudformation-cli): The CloudFormation Provider Development Toolkit allows you to author your own resource providers that can be used by CloudFormation.
- [cloudformation-cli-go-plugin](https://github.com/aws-cloudformation/cloudformation-cli-go-plugin): The CloudFormation Provider Development Toolkit Go Plugin allows you to autogenerate Go code based on an input schema.
- [cloudformation-cli-java-plugin](https://github.com/aws-cloudformation/cloudformation-cli-java-plugin): The CloudFormation Provider Development Toolkit Java Plugin allows you to autogenerate Java code based on an input schema.
- [cloudformation-cli-python-plugin](https://github.com/aws-cloudformation/cloudformation-cli-python-plugin): The CloudFormation Provider Development Toolkit Python Plugin allows you to autogenerate Python code based on an input schema.
- [custom-resource-helper](https://github.com/aws-cloudformation/custom-resource-helper): Simplify best practice Custom Resource creation, sending responses to CloudFormation and providing exception, timeout trapping, and detailed configurable logging.

## Public Coverage Roadmap

The Public Coverage Roadmap is supported by the AWS CloudFormation team to help prioritise coverage work streams and resource improvements.

- [aws-cloudformation-coverage-roadmap](https://github.com/aws-cloudformation/aws-cloudformation-coverage-roadmap): This is a public roadmap focused on upcoming coverage support for CloudFormation. Coverage prioritisation is influenced by contributions and feedback to this roadmap.

## Blog Posts & Talks

Our community is our most powerful tool, and the following are hand picked submissions from some of our favourite contributors.

- [YAML Is Better than Your Favorite Language: Fightin' words about Infrastructure as code](https://acloud.guru/series/serverlessconf-nyc-2019/view/yaml-better) by Ben Kehoe
- [AWS CloudFormation Custom Resource Types: A Walkthrough](https://onecloudplease.com/blog/aws-cloudformation-custom-resource-types-a-walkthrough) by Ian McKay

## Documentation

CloudFormation's [public documentation](https://docs.aws.amazon.com/cloudformation/) is also open-sourced and we love to accept contributions.

- [cloudformation-user-guide](https://github.com/awsdocs/aws-cloudformation-user-guide): CloudFormation's public documentation source repository
- [aws-cfn-resource-specs](https://github.com/ScriptAutomate/aws-cfn-resource-specs): A Completely Tracked, Versioned, and Audited Collection Store of CloudFormationResource.json Specification Files. These are the specification files created by AWS and ingested by tools wrapped around CloudFormation template development, such as most tools listed under the [Code Generation](#code-generation) section. The repository includes detailed, automatically generated changelogs about each new release, such as information on new resource types and what regions support them.

## Contribute

Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.

## License Summary

This sample code is made available under a modified MIT license. See the LICENSE file.
