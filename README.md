# Chaos Imp AWS IAM Policies

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/gitbucket/gitbucket/blob/master/LICENSE)

This repository contains AWS IAM policies for Chaos Imp—a framework for creating, executing, and running [chaos engineering](https://principlesofchaos.org/) (CE) experiments on AWS.

## ImpFis.json

Add this policy to an IAM role, so Chaos Imp is able to create experiment templates. Once the role is created, set its ARN in Chaos Imp config:

```bash
imp config set TemplateRoleArn <ROLE_ARN>
```

## ImpSsm.json

Add this policy to an IAM role and attach it to EC2 instances that are part of your experiments.