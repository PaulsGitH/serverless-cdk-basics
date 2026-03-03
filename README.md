# serverless-cdk-basics

Infrastructure as Code project built with AWS CDK v2 and TypeScript. This repository provisions a minimal serverless backend using AWS Lambda and DynamoDB, focusing on core CDK patterns, IAM permissions, and repeatable stack deployment.

## Architecture Overview

This stack provisions:

- AWS Lambda function using NodejsFunction bundling
- DynamoDB table for persistent storage
- IAM permissions defined using CDK grant helpers
- Stack outputs for service access

The design is intentionally minimal to demonstrate clean infrastructure definition and lifecycle management.

## Technology Stack

- AWS CDK v2
- TypeScript
- AWS Lambda
- DynamoDB
- AWS SDK v3

## Repository Structure

- bin  
  CDK application entry point

- lib  
  CDK stack definitions

- lambdas  
  Lambda handler implementations

- seed and shared  
  Seed data and shared utilities when applicable

## Installation

npm install

## Deployment

cdk deploy

The deployment process synthesises and provisions all infrastructure resources defined in the stack.

## Stack Lifecycle Management

To remove all provisioned infrastructure and avoid unnecessary cost:

cdk destroy

## Key Concepts Demonstrated

- Declarative infrastructure with AWS CDK
- Lambda deployment using CDK NodejsFunction
- DynamoDB table provisioning
- IAM least privilege via CDK grants
- Repeatable environment provisioning
