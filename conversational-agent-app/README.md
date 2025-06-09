---
title: "Conversational Agent App"
language: python
author: "Vivian Xie"
date: 2025-06-09
---

# Conversational Agent App


![](./assets/genie_room0.png)
![](./assets/genie-space.png)
![](./assets/genie-space4.png)

This repository demonstrates how to integrate Databricks' AI/BI Genie Conversation APIs into custom Databricks Apps applications, allowing users to interact with their structured data using natural language.

You can also click the Generate insights button and generate deep analysis and trends of your data.
![](./assets/insights1.png)
![](./assets/insights2.png)



## Overview

This app is a Dash application featuring a chat interface powered by Databricks Genie Conversation APIs, built specifically to run as a Databricks App. This integration showcases how to leverage Databricks' platform capabilities to create interactive data applications with minimal infrastructure overhead.

The Databricks Genie Conversation APIs (in Public Preview) enable you to embed AI/BI Genie capabilities into any application, allowing users to:
- Ask questions about their data in natural language
- Get SQL-powered insights without writing code
- Follow up with contextual questions in a conversation thread

## Key Features

- **Powered by Databricks Apps**: Deploy and run directly from your Databricks workspace with built-in security and scaling
- **Zero Infrastructure Management**: Leverage Databricks Apps to handle hosting, scaling, and security
- **Workspace Integration**: Access your data assets and models directly from your Databricks workspace
- **Natural Language Data Queries**: Ask questions about your data in plain English
- **Stateful Conversations**: Maintain context for follow-up questions

## Example Use Case

This demo shows how to create a simple interface that connects to the Genie API, allowing users to:
1. Start a conversation with a question about their supply chain data
2. View generated SQL and results
3. Ask follow-up questions that maintain context

## Deploying to Databricks apps

1. Clone the repository to workspace directory such as 
/Workspace/Users/wenwen.xie@databricks.com/genie_space
```bash
git clone https://github.com/databrickslabs/sandbox.git
```
![](./assets/genie-space1.png)


2. Deploy the app using the Databricks Apps interface:
   - Clone the repository to your Databricks workspace.
   - Navigate to the **Apps** tab in the sidebar.
   - Click on your app in the **Name** column.
   - Click **Deploy** and select the folder 'conversational-agent-app' from the cloned repository.
   - Click **Select**, then **Deploy**.
   - Review the configuration and click **Deploy**.

For more details, refer to the [official Databricks documentation](https://docs.databricks.com/aws/en/dev-tools/databricks-apps/deploy).

3. Troubleshooting issues:
   
   For trouble shooting, navigate to the genie room monitoring page and check if the query has been sent successfully to the genie room via the API. 

![](./assets/troubleshooting1.png)

   Click open the query and check if there is any error or any permission issues.


![](./assets/troubleshooting2.png)


## Resources

- [Databricks Genie Documentation](https://docs.databricks.com/aws/en/genie)
- [Conversation APIs Documentation](https://docs.databricks.com/api/workspace/genie)
- [Databricks Apps Documentation](https://docs.databricks.com/aws/en/dev-tools/databricks-apps/)