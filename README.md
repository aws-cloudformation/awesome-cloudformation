## Awesome CloudFormation [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of resources and projects for working with [AWS CloudFormation](https://aws.amazon.com/cloudformation/).

## Contents

- [Awesome CloudFormation <img src="https://awesome.re/badge.svg" alt="Awesome">](#awesome-cloudformation-img-src%22httpsawesomerebadgesvg%22-alt%22awesome%22)
- [Contents](#contents)
- [CloudFormation Samples](#cloudformation-samples)
  - [Templates](#templates)
  - [Modules](#modules)
  - [Resource Types](#resource-types)
  - [Hooks](#hooks)
- [Authoring and Testing Tools](#authoring-and-testing-tools)
- [CLI Tools](#cli-tools)
- [Code Generation](#code-generation)
- [Custom Resource Development](#custom-resource-development)
- [Third Party Resource Types](#third-party-resource-types)
- [Third Party Hooks](#third-party-hooks)
- [Public Coverage Roadmap](#public-coverage-roadmap)
- [Blog Posts and Talks](#blog-posts-and-talks)
- [Documentation](#documentation)
  - [Reference Guides](#reference-guides)
    - [AWS](#aws)
    - [3rd parties](#3rd-parties)
- [Contribute](#contribute)
- [License Summary](#license-summary)

## CloudFormation Samples

The following are pre-built CloudFormation Samples demonstrating how to use AWS CloudFormation to construct various canned resources, modules, applications or resource groupings.

### Templates
- [aws-cf-templates](https://github.com/widdix/aws-cf-templates): Free Templates for AWS CloudFormation
- [aws-cloudformation-templates](https://github.com/awslabs/aws-cloudformation-templates): Sample AWS CloudFormation templates which are intended to support learning how to declare specific AWS resources or solve particular use cases.
- [aws-quickstart](https://github.com/aws-quickstart): Automated gold-standard deployments on AWS
- [asecure.cloud](https://asecure.cloud/): A free repository of customizable AWS security configurations and best practices

### Modules
- [aws-cloudformation-samples](https://github.com/aws-cloudformation/aws-cloudformation-samples/tree/main/modules): Reusable CloudFormation modules to jump start your collection.

### Resource Types
- [aws-cloudformation-samples](https://github.com/aws-cloudformation/aws-cloudformation-samples/tree/main/resource-types): Sample CloudFormation Resource Types

### Hooks
- [aws-cloudformation-samples](https://github.com/aws-cloudformation/aws-cloudformation-samples/tree/main/hooks): Sample CloudFormation Hooks

## Authoring and Testing Tools

These tools are designed to assist in the authoring and testing process for AWS CloudFormation. Tools include template generation, linting and testing applications.

- [AWSConsoleRecorder](https://github.com/iann0036/AWSConsoleRecorder): Records actions made in the AWS Management Console and outputs the equivalent CLI/SDK commands and CloudFormation/Terraform templates.
- [Former2](https://github.com/iann0036/former2): Generate CloudFormation / Terraform / Troposphere templates from your existing AWS resource
- [cfn-python-lint](https://github.com/aws-cloudformation/cfn-python-lint): Validate CloudFormation yaml/json templates against the CloudFormation spec and additional checks. Includes checking valid values for resource properties and best practices.
- [cfn-guard](https://github.com/aws-cloudformation/cloudformation-guard): A set of tools to check AWS CloudFormation templates for policy compliance using a simple, policy-as-code, declarative syntax
- [Visual Studio Code extension](https://github.com/aws-cloudformation/aws-cfn-lint-visual-studio-code): CloudFormation Linter integration, autocompletion, reference documentation links on hover
- [cfn_nag](https://github.com/stelligent/cfn_nag): The cfn-nag tool looks for patterns in CloudFormation templates that may indicate insecure infrastructure.
- [taskcat](https://github.com/aws-quickstart/taskcat): taskcat is a tool that tests AWS CloudFormation templates. It deploys your AWS CloudFormation template in multiple AWS Regions and generates a report with a pass/fail grade for each region.
- [org-formation](https://github.com/OlafConijn/AwsOrganizationFormation): a tool that helps you write CloudFormation for your AWS Organization resources and create links between regular cloudformation resources across your accounts and regions.
- [cfn checklist](https://cfnchecklist.com/): a list of of things to look out for before launching your infrastructure to production.
- [cfn flip](https://cfnflip.com/): a tool that converts AWS CloudFormation templates between JSON and YAML formats.
- [cfn-diagram](https://github.com/mhlabs/cfn-diagram): CLI tool to visualise CloudFormation templates as diagrams.
- [cfsec](https://cfsec.dev): CloudFormation static analysis to identify potential misconfigurations before they reach production.

## CLI Tools

This section contains tools which have been designed to improve the experience of interacting with the CloudFormation service through a terminal session.

- [awscfncli](https://github.com/Kotaimen/awscfncli): awscfncli helps build and manage complex AWS CloudFormation stacks.
- [stacker](https://github.com/cloudtools/stacker): An AWS CloudFormation Stack orchestrator/manager.
- [sceptre](https://github.com/Sceptre/sceptre): Sceptre is a tool to drive AWS CloudFormation. It automates the mundane, repetitive and error-prone tasks, enabling you to concentrate on building better infrastructure.
- [cfn-teardown](https://github.com/nirdosh17/cfn-teardown): Cleanup CloudFormation stacks respecting the order of dependencies.
- [rain](https://github.com/aws-cloudformation/rain): A command line tool for working with AWS CloudFormation. It has tools for creating, comparing, and formatting templates and a pleasant CLI experience for creating, updating, and deleting stacks.

## Code Generation

If you prefer imperative coding, or just using your favourite programming language, the following projects are intended to abstract the creation of AWS CloudFormation templates.

- [aws-cdk](https://github.com/aws/aws-cdk): The AWS Cloud Development Kit (AWS CDK) is an open-source software development framework to define cloud infrastructure in code and provision it through AWS CloudFormation.
- [serverless-application-model](https://github.com/awslabs/serverless-application-model): The AWS Serverless Application Model (SAM) is an open-source framework for building serverless applications. It provides shorthand syntax to express functions, APIs, databases, and event source mappings. With just a few lines of configuration, you can define the application you want and model it.
- [eksctl](https://github.com/weaveworks/eksctl): A CLI tool that uses CloudFormation to create clusters on EKS.
- [mu](https://github.com/stelligent/mu): Similar to how the Serverless Framework improved the developer experience of Lambda and API Gateway, this tool makes it easier for developers to use EKS or ECS as a microservices platform.
- [OpenJS Architect](https://github.com/architect/architect): Generate AWS CloudFormation and AWS Serverless Application Model code from a very terse and friendly high level manifest file written in `JSON`, `YAML`, `TOML` or `.arc` format
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

## Third Party Resource Types

The following third-party vendors have created resource types using the CloudFormation CLI and can be downloaded and added to your accounts via the Registry.

- [Atlassian](https://github.com/opsgenie/opsgenie-cloudformation-resources) Creates Atlassian::Opsgenie::User, Atlassian::Opsgenie::Team, and Atlassian::Opsgenie::Integration
- [Datadog](https://github.com/DataDog/datadog-cloudformation-resources#resources-available) Creates Datadog::Integrations::AWS, Datadog::Monitors::Monitor, Datadog::Monitors::Downtime, and Datadog::IAM::User
- [Densify](https://github.com/densify-dev/cloudformation-optimization-as-code) Creates Densify::Optimization::Recommendation
- [Dynatrace](https://github.com/mnalezin/DynatraceInstallerAgent) Creates Dynatrace::Installer::Agent
- [Fortinet](https://github.com/fortinet/aws-cloudformation-resource-provider) Creates Fortinet::FortiGate::SystemAdmin, Fortinet::FortiGate::SystemDns, and Fortinet::FortiGate::SystemInterface
- [NewRelic](https://github.com/newrelic/cloudformation-partner-integration) Creates NewRelic::Alerts::NrqlAlert
- [Spotinst](https://github.com/spotinst/spotinst-aws-cloudformation-registry) Creates Spotinst::Elastigroup::Group

## Third Party Hooks

- [Open Policy Agent](https://github.com/StyraInc/opa-aws-cloudformation-hook) Hook to allow policy-based decisions on stacks using [Open Policy Agent](https://www.openpolicyagent.org/)

## Public Coverage Roadmap

The Public Coverage Roadmap is supported by the AWS CloudFormation team to help prioritise coverage work streams and resource improvements.

- [aws-cloudformation-coverage-roadmap](https://github.com/aws-cloudformation/aws-cloudformation-coverage-roadmap): This is a public roadmap focused on upcoming coverage support for CloudFormation. Coverage prioritisation is influenced by contributions and feedback to this roadmap.

## Blog Posts and Talks

Our community is our most powerful tool, and the following are hand picked submissions from some of our favourite contributors.

- [YAML Is Better than Your Favorite Language: Fightin' words about Infrastructure as code](https://acloud.guru/series/serverlessconf-nyc-2019/view/yaml-better) by Ben Kehoe
- [AWS CloudFormation Custom Resource Types: A Walkthrough](https://onecloudplease.com/blog/aws-cloudformation-custom-resource-types-a-walkthrough) by Ian McKay
- [The OPA AWS CloudFormation Hook](https://blog.styra.com/blog/the-opa-aws-cloudformation-hook)

## Documentation

### Reference Guides
#### AWS
CloudFormation's [public documentation](https://docs.aws.amazon.com/cloudformation/) is also open-sourced and we love to accept contributions.

- [cloudformation-user-guide](https://github.com/awsdocs/aws-cloudformation-user-guide): CloudFormation's public documentation source repository
- [aws-cfn-resource-specs](https://github.com/ScriptAutomate/aws-cfn-resource-specs): A Completely Tracked, Versioned, and Audited Collection Store of CloudFormationResource.json Specification Files. These are the specification files created by AWS and ingested by tools wrapped around CloudFormation template development, such as most tools listed under the [Code Generation](#code-generation) section. The repository includes detailed, automatically generated changelogs about each new release, such as information on new resource types and what regions support them.
- [AWS CloudFormation Workshop](https://cfn101.workshop.aws/): A workshop that takes you through CloudFormation from the beginning up to more advanced topics.

#### 3rd parties
- [Scale Your CloudFormation](https://github.com/jeshan/scale-your-cloudformation): An in-depth guide for intermediate users on becoming successful with Infrastructure as Code on AWS

## Contribute

Contributions welcome! Read the [contribution guidelines](CONTRIBUTING.md) first.

## License Summary

This sample code is made available under a modified MIT license. See the LICENSE file.
