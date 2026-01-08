Understanding how to use AI responsibly in technical writing is essential. AI can be a powerful assistant, but it cannot replace human writers. Instead, it should be used to reduce repetitive work and create space for higher-value tasks.

In this case, I explored which parts of the documentation workflow could be automated so I could focus more on writing conceptual content and creating high-quality CLI, JSON, and AWS CloudFormation examples.

These solutions were created for Amazon ECS, but are generic for other AWS services.

## Connecting documentation with the code

Amazon ECS uses identity-based policies as one of its core security mechanisms. It also provides a set of managed policies that grant specific permissions for customers.

To document these policies, I used the Amazon Q CLI with MCP servers to read permissions directly from the submitted code and automatically generate documentation. This approach provided several benefits:

- Ensured the documentation stayed synchronized with the source code
- Reduced manual effort and the risk of errors
- Streamlined updates when permissions changed

Live Documentation: [AmazonECSInstanceRolePolicyForManagedInstances](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/security-iam-awsmanpol.html#security-iam-awsmanpol-AmazonECSInstanceRolePolicyForManagedInstances)


---

## Figma to tasks

Figma mock-ups are often used as starting points. For documentation, the mock-ups map to tasks that provide instructions for a job.

To document these tasks, I used the Amazon Q CLI with MCP servers to read the mock-ups from Figma, and then create a task following a defined DITA pattern. This approach provided several benefits:

- Ensured the documentation stayed synchronized with the mock-ups
- Reduced manual effort and the risk of errors
- Streamlined updates when strings changed



Live Documentation: [Creating an Amazon ECS blue/green deployment](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ManagedInstances.html)
