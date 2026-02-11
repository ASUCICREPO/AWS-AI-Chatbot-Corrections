# AWS AI Chatbot for Corrections - Amazon Q Business with Web Crawler

This project deploys an Amazon Q Business application with a web crawler data source. The solution enables you to create an enterprise search and generative AI assistant that can crawl, index, and retrieve information from specified websites.

Amazon Q Business is the most capable generative AI-powered assistant for finding information, gaining insight, and taking action at work. It makes generative AI securely accessible to everyone in your organization and helps your employees get work done faster.

## Disclaimers
Customers are responsible for making their own independent assessment of the information in this document.

This document:

(a) is for informational purposes only,

(b) references AWS product offerings and practices, which are subject to change without notice,

(c) does not create any commitments or assurances from AWS and its affiliates, suppliers or licensors. AWS products or services are provided "as is" without warranties, representations, or conditions of any kind, whether express or implied. The responsibilities and liabilities of AWS to its customers are controlled by AWS agreements, and this document is not part of, nor does it modify, any agreement between AWS and its customers, and

(d) is not to be considered a recommendation or viewpoint of AWS.

Additionally, you are solely responsible for testing, security and optimizing all code and assets on GitHub repo, and all such code and assets should be considered:

(a) as-is and without warranties or representations of any kind,

(b) not suitable for production environments, or on production or other critical data, and

(c) to include shortcuts in order to support rapid prototyping such as, but not limited to, relaxed authentication and authorization and a lack of strict adherence to security best practices.

All work produced is open source. More information can be found in the GitHub repo.

## Deployment Options

You can deploy this solution using one of two methods:

- **[Infrastructure as Code (IaC) Deployment](docs/iac-deployment.md)** - Automated deployment using AWS CDK (Recommended)
- **[Manual Deployment](docs/manual-deployment.md)** - Step-by-step manual setup through AWS Console

## Architecture Overview

This solution deploys the following AWS resources:

- **Amazon Q Business Application**: The core Q Business application that provides the generative AI capabilities
- **Amazon Q Business Index**: A starter index to store and search document content
- **Amazon Q Business Retriever**: A native index retriever to search indexed content
- **Amazon Q Business Web Experience**: A web interface for users to interact with the Q Business application
- **Amazon Q Business Web Crawler Data Source**: A web crawler that indexes content from specified seed URLs
- **IAM Roles and Policies**: Necessary permissions for the Q Business services to operate
- **KMS Key**: For encryption of sensitive data

## What You'll Need

- AWS Account with appropriate permissions
- AWS Identity Center set up and configured
- List of websites you want to crawl and index

## Documentation

- **[IaC Deployment Guide](docs/iac-deployment.md)** - Complete guide for automated deployment
- **[Manual Deployment Guide](docs/manual-deployment.md)** - Step-by-step manual setup instructions

## License

This project is licensed under the MIT License - see the LICENSE file for details.
